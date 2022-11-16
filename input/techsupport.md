title: Learning path
header: One possible suggested learning path
menu-position: 64
indent: 1

---

Once you've read [the previous page about what a file is](filesys.html),
you can start learning more about the details.
(Dumb math analogy: before studying math olympiad seriously,
you should have seen enough that you can tell the difference
between a geometry problem and a functional equation.)

## {{ hl("path", "Evan's suggested learning path") }}

If I was personally teaching computer literacy,
I would break it down into the following steps
(this is obviously not the only layout):

1. Learning how to use a command prompt to navigate files and folders
   in a terminal, and execute commands.
   You can learn this in a day or two from [Zed Shaw][term]
   or [missing.csail.mit.edu][missing- csail] or [djangogirls][term2] or
   whatever you find on Google.
2. Find a text editor you like (as stated, any text editor opens any plain
   text file). Be able to open, edit, and save an arbitrary text file. (This
   is likely to be covered in step 1 already; LaTeX users may also know this
   step already.)
3. You should then learn your first programming language. The hardest part!

## {{ hl("language", "Picking a language") }}

In programming culture, choices of language draw the same visceral reactions as
discussions about race and religion.
That said, among languages I have used at least a little bit,
here is Evan's tier list:

1. [Python][python]: reads like English, simple to learn, and Evan's native language.
   This is my personally recommended first language.
   The main downside is that it is a lot slower.
   I grew up on [this Python book](http://openbookproject.net/thinkcs/python/english3e/index.html)
   and recommend it;
   there are [tons of other free Python tutorials][nonpro].
   (Note for experts: Python doesn't have type safety by default, but it can.)

2. [TypeScript][typescript]: It actually compiles _to_ JavaScript,
   i.e. there is a program that accepts TypeScript input
   and produces JavaScript output.
   Besides that, it has some similarity to Python,
   but as its name suggests has stricter type safety.

3. [C++][cpp]: Much faster than Python, but harder to read and write.
   However, if you want to do
   [competitive programming](https://ioinformatics.org/)
   then you probably want to use this one.

4. [Java][java]: It's a pretty wordy language.
   I don't personally like it much, but I can see the appeal.
   The main reason it's still relevant to kids today is because
   of AP Computer Science A,
   but that class does a pretty bad job of teaching it anyway.

5. [JavaScript](https://www.destroyallsoftware.com/talks/wat):
   Please no.[^js] Use TypeScript instead.
   (Longer argument on [blog](https://blog.evanchen.cc/?p=1437).)

6. [PHP](https://eev.ee/blog/2012/04/09/php-a-fractal-of-bad-design/):
   Definitely no.

[python]: https://www.python.org/
[typescript]: https://www.typescriptlang.org/
[cpp]: https://en.wikipedia.org/wiki/C%2B%2B
[java]: https://en.wikipedia.org/wiki/Java_(programming_language)

Second-hand, I've also heard a lot of good things about [Go](https://go.dev/).

Sidenote: HTML and LaTeX are
[markup languages](https://stackoverflow.com/a/145179),
and not programming languages in practice.
(Pedants may argue they are _technically_ Turing-complete
if abused enough, but why would you do that?)
CSS is not a programming language either for similar reasons.

## {{ hl("advanced", "Advanced stuff (skip for now)") }}

Some other advanced things you can do involve
learning [git](https://duckduckgo.com/?q=git+tutorial),
switching to Linux, and learning an advanced text editor like
[Vim](https://www.vim.org) or
[Emacs](https://en.wikipedia.org/wiki/Emacs).
I'm not going to talk about the expert stuff here for brevity.
For now, your job is to pick a language and mess with it.

Once you've done that you can check
[FAQs on Linux](faq-linux.html) for elaborations on the advanced stuff.

[^js]:
    The reason I specifically anti-recommend PHP and vanilla JavaScript is
    that as a beginner I think you shouldn't get in the habit of writing code like
    `"You have " + n + " dollars"` when you are first starting out.
    (Okay, I also hate both languages, but that's unrelated.)

## {{ hl("euler", "Shout-out to Project Euler") }}

I have lots and lots of love for
[Project Euler](https://projecteuler.net/about).
This is an enormous collection of problems that require both
programming ability and problem-solving math ability in order to solve.
I think if you are new to programming but have math background,
this is a great way to start off!
It can change the way you think about both fields.

If you do choose to play, you may start with some of the later levels,
the first 35 levels or so are fairly easy,
and later levels are more interesting.

[term]: https://learnpythonthehardway.org/python3/appendixa.html
[term2]: https://tutorial.djangogirls.org/en/intro_to_command_line/
[nonpro]: https://wiki.python.org/moin/BeginnersGuide/NonProgrammers
[missing-csail]: https://missing.csail.mit.edu/
