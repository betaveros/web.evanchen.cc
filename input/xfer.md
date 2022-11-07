title: XFER
header: evanchen.cc XFER
description: Evan is sending you a file.

---

<div class="alert alert-secondary" id="output">
<h3 class="alert-heading">Hello hello hey</h3>
Evan Chen is sending you a private file,
<a href="https://youtu.be/ChTGq3o9D6c">isn't that great</a>?
</div>

<hr />

<div class="form-group">
<label for="xfer_filename"><h3>Filename</h3></label>
<input class="form-control" style="font-family:Inconsolata,monospace;" id="xfer_filename"></input>
</label>
</div>
<div>
<label for="xfer_password"><h3>Password</h3></label>
<input type="password" class="form-control" id="xfer_password"></input>
</label>
<hr />
<button class="btn btn-primary">Unlock</button>
</div>
<script type="text/javascript">
$(() => {

	async function digestMessage(message) {
		const msgUint8 = new TextEncoder().encode(message);
		const hashBuffer = await crypto.subtle.digest('SHA-512', msgUint8);
		const hashArray = Array.from(new Uint8Array(hashBuffer));
		const hashHex = hashArray.map(b => b.toString(16).padStart(2, '0')).join('');
		return hashHex;
	}
	const url = new URL(window.location.href);
	const init_filename = url.searchParams.get('f');
	const target = url.searchParams.get('h');
	const salt = url.searchParams.get('s') || '';
	if (init_filename) {
		$("#xfer_filename").val(init_filename);
	}

	$("#xfer_password").on('focusout', async () => {
		const filename = $("#xfer_filename").val();
		const password = $("#xfer_password").val();
		const kludge = 'evanchen.cc/xfer|' + filename + '|' + salt + '|' + password;
		const h1 = await digestMessage(kludge);
		const h3 = await digestMessage(h1);
		const checksum = h3.slice(0,6);
		if (password === "") {
			$("#output").removeClass();
			$("#output").addClass("alert alert-warning");
			$("#output").html(
				`<h3 class="alert-heading">Aloha</h3>`
				+ `Type the filename and password (both required).`
			);
		} else if (target && target !== checksum && filename === init_filename) {
			$("#output").removeClass();
			$("#output").addClass("alert alert-danger");
			$("#output").html(
				`<h3 class="alert-heading">Wrong!</h3>`
				+ `You entered an invalid password, try again.`
			);
		} else if (!target) {
			$("#output").removeClass();
			$("#output").addClass("alert alert-primary")
			$("#output").html(
				`<h3 class="alert-heading">Here you go!</h3>`
				+ `<a href="xfer-payload/${h1}" `
				+ `download="${filename}" class="alert-link">`
				+ `Download now (checksum ${checksum})</a>. `
				+ `If you get a 404 error, check the password.`
			);
		} else {
			$("#output").removeClass();
			$("#output").addClass("alert alert-success")
			$("#output").html(
				`<h3 class="alert-heading">Success!</h3>`
				+ `<a href="xfer-payload/${h1}" `
				+ `download="${filename}" class="alert-link">`
				+ `Download now</a>.`
			);
		}

	});
});
</script>
