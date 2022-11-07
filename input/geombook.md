title: EGMO book
menu-position: 71
header: Euclidean Geometry in Mathematical Olympiads (EGMO)
indent: 1
description: Synopsis and errata for EGMO geometry textbook for math olympiad students.

---

<span style="float:left;padding:10px;">
[![Book cover][cover]][ebook]
</span>

<span style="color:red; font-size: 120%;">
**You can get a hard copy from [Amazon][amazon] or [the AMS][hardcopy].
You can also [purchase a PDF][ebook].**
</span>

*Euclidean Geometry in Mathematical Olympiads* (often abbreviated *EGMO*,
despite an olympiad having the [same name][girls])
is a comprehensive problem-solving book in Euclidean geometry.
It was written for competitive students training for national
or international mathematical olympiads.
However, it has no prerequisites other than a good deal of courage:
any student with proof experience
should be able to follow the exposition.
The book contains a selection of about 300 problems from around the world
and is accompanied by about 250 figures.

I wrote this textbook while
[serving time as a high school clerk][fillblank].
You can [read about the publication process][publishing].

## {{ hl("prereq", "Prerequisites and material") }}

There are essentially no geometry prerequisites;
EGMO is **entirely self-contained**.
(This was one of the design goals.)
The main limiting factor is instead the ability to **read proofs**;
as long as you can follow mathematical arguments,
then you should be able to follow the exposition
even if you don't know any geometrical theorems.
Here is a freely available subset of the book:

* [Table of contents][toc].
* [Chapter 2 (Circles)][egmo2] and [Chapter 8 (Inversion)][egmo8]
	(available for free).
* [Chapters 1-3][googlebook] on Google Books preview.
* *Parody version of entire book*: check out
	[Undergraduate Math 011: a firsT yeaR coursE in geometrY](textbooks/tr011ey.pdf),
	made for April Fool's Day 2019.

## {{ hl("errata", "Errata (aka selected solutions to Problem 11.0)") }}

Here is a [list of all mistakes that I am aware of.](upload/geombook-errata.pdf)
Most mistakes are harmless, but a few of the mistakes are significant;
the important ones are reproduced here, too.

+ On **page 12**, Theorem 1.22, the four points could also be collinear.
+ On **page 76**, Theorem 5.1 is missing a factor of $\frac12$.
+ On **page 92**, Problem 5.23, when defining $G$, line $HE$ should intersect
	$\Gamma_1$, not $\Gamma_2$.
+ On **page 107**, the proof of part (a) of the theorem
	has several issues, and is probably best to just ignore.
	Figure 6.6B is also broken.
	(The result is still true, and the proof of part (b) is correct.)
+ On **page 145**, Problem 7.44, change the angle condition to $\measuredangle BC\_1A\_1 = \measuredangle ACB = \measuredangle B\_1C\_1A$.
+ On **page 146**, Problem 7.52, change $\angle PCB$ to $\angle PBC$.
+ On **page 159**, in Lemma 8.16, change "fixes $B$ and $C$" to "swaps $B$ and $C$".
+ On **page 184**, in Theorem 9.33, uniqueness is not true for (b) or (c).
	The last sentence is also wrong as written.
	The correct sentence is: if the *circumcircle* of a cyclic quadrilateral is preserved,
	then so is the cross ratio of the cyclic quadrilateral.
+ On **page 243**, Solution 1.50 is incomplete; one also needs to check $A$, $P$, $W$ are collinear.
	Thus, add the remark $\measuredangle NPA = \measuredangle NMA = \measuredangle NMC = \measuredangle NBC = \measuredangle NBW = \measuredangle NPW$.
	(Radical axis also works.)
+ On **page 268**, Solution 7.44 is completely broken; it's solving a different
	problem. See the above file for a fixed solution.
+ On **page 274**, Solution 8.37 is wrong, it assumes $AB$ passes through the center of $\omega\_2$.

## {{ hl("solutions", "On solutions to problems") }}

I included solutions to about a quarter of the
practice problems in the back of the textbook
(it was impossible to include more for space reasons).
If you are stuck on a problem for which no solution is provided,
here are some possible places to look:

1. Each problem in the text has one or more hints,
	the intention is that the union of all the hints
	should form an outline of the complete solution
	(even if the details are omitted).

2. There is a [user-created forum][userforum]
	which has a link to discussion for every problem.

3. I included sources for as many of the problems as possible,
	so looking up the corresponding thread on
	[Art of Problem Solving's Contest Index][contests]
	will generally yield a solution to any sourced problem.
	(The search function can work too, but is usually less helpful.)

4. If all of the above fail, try posting on the AoPS forums directly.

[userforum]: https://artofproblemsolving.com/community/c618937h1605831_egmo_problem_discussions_links

## {{ hl("resources", "More resources") }}

Of course there are other good geometry textbooks too.
A few that I recommend are:

* [106][106], [107][107], and [110][110] Geometry Problems
* [A Beautiful Journey Through Olympiad Geometry][stefan], which is pay-what-you-want!
* [Lemmas in Olympiad Geometry][LOG]
* [UKMT Plane Euclidean Geometry][ukmt], but consider starting from Chapter 3

See also [advice from Geoff Smith on geometry](https://people.bath.ac.uk/masgcs/geo.pdf).

[106]: https://www.awesomemath.org/product/106-geometry-problems-from-amsp/
[107]: https://www.awesomemath.org/product/107-geometry-problems-from-amy/
[110]: https://bookstore.ams.org/xyz-14/
[LOG]: https://www.awesomemath.org/product/lemmas-in-olympiad-geometry/
[stefan]: https://www.olympiadgeometry.com/
[ukmt]: https://shop.ukmt.org.uk/ukmt-books/plane-euclidean-geometry


[ebook]: https://bookstore.ams.org/prb-27/
[cover]: https://www.maa.org/sites/default/files/images/ebooks/problem_books/EGMO.png
[egmo2]: https://www.maa.org/sites/default/files/pdf/ebooks/pdf/EGMO_chapter2.pdf
[egmo8]: https://www.maa.org/sites/default/files/pdf/ebooks/pdf/EGMO_chapter8.pdf
[googlebook]: https://books.google.com/books?id=47UaDAAAQBAJ&lpg=PP1&pg=PP1#v=onepage&q&f=false
[amazon]: https://smile.amazon.com/Euclidean-Geometry-Mathematical-Olympiads-Problem/dp/0883858398?ie=UTF8&*Version*=1&*entries*=0
[hardcopy]: https://bookstore.ams.org/prb-27/
[girls]: https://www.egmo.org/
[contests]: https://artofproblemsolving.com/community/c13_contests

[fillblank]: https://blog.evanchen.cc/2016/05/27/fill-in-the-blank/
[publishing]: https://blog.evanchen.cc/2016/11/11/notes-on-publishing-my-textbook/
[toc]: https://www.maa.org/sites/default/files/pdf/pubs/books/EGMO_TOC.pdf
