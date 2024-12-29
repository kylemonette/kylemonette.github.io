---
title: 'Vampire Matrices'
date: 2024-12-29
permalink: /posts/2024/12/vampire-matrices/
tags:
  - Vampire Matrices
---


On Halloween in 2020, Matt Parker of the YouTube Channel *Standup Maths* posted a [video](https://www.youtube.com/watch?v=9nogAYHmnNw) about *Vampire Matrices*. In this early definition of the term, Parker defined a (single) Vampire Matrix to be a square matrix consisting of positive integers such that the square of the matrix is equal to its element-wise concatenation. As a $2\times 2$ example,
\\[
\mat{cc}
3 & 4 \\\\ 6 & 8
\rix^2 = 
\mat{cc}
33 & 44 \\\\ 66 & 88
\rix
\\]
and a $3\times 3$ example,
\\[
\mat{ccc}
1 & 3 & 1 \\\\ 3 & 9 & 3 \\\\ 1 & 3 & 1
\rix^2 =
\mat{ccc}
11 & 33 & 11 \\\\\\
33 & 99 & 33 \\\\\\
11 & 33 & 11
\rix.
\\] As Parker illustrates in his video, himself and a small group of other YouTube mathematicians noticed that these matrices satisfy the equation
\\[
A^2 = 11 A
.\\]
If we allow for two-digit integer entries (by this I mean *strictly* two-digit numbers to rule out things like $04$ which is really just $4$, a one digit number), then the matrix equation of interest becomes
\\[
A^2 = 101 A
.\\] One such matrix is
\\[
\mat{cc}
60 & 30 \\\\ 82 & 41 \rix^2 = \mat{cc} 6060 & 3030 \\\\ 8282 & 4141 \rix
\\]