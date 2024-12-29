---
title: 'Vampire Matrices'
date: 2024-12-29
permalink: /posts/2024/12/vampire-matrices/
tags:
  - Vampire Matrices
---


On Halloween in 2020, Matt Parker of the YouTube Channel *Standup Maths* posted a [video](https://www.youtube.com/watch?v=9nogAYHmnNw) about *Vampire Matrices*. In this early definition of the term, Parker defined a (single) Vampire Matrix to be a square matrix consisting of positive integers such that the square of the matrix is equal to its element-wise concatenation. As an example,
\\[
\mat{cc}
3 & 4 \\\\ 6 & 8
\rix^2 = 
\mat{cc}
33 & 44 \\\\ 66 && 88
\rix, \qquad
\mat{ccc}
1 & 3 & 1 \\\\
3 & 1 & 3 \\\\
1 & 3 & 1
\rix^2 = \mat{ccc}
11 & 33 & 11 \\\\
33 & 11 & 33 \\\\
11 & 33 & 11
\rix
\\]