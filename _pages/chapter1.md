---
layout: single
title: "Chapter 1"
permalink: /215/chapter1/
author_profile: true
---

## Interests

I am interested in topics in numerical linear algebra, primarily in Krylov subspace methods. Initially we were interested in augmentation and restarting methods for GMRES, and have recently been switching to the symmetric eigenvalue problem and SVD computations. In the future, we hope to dip more into the randomized NLA algorithms that are in the spotlight right now.

## Project: Vampire Matrices

Recently I have been exploring a special type of matrices sometimes called <i>vampire matrices</i>, which became popular from Matt Parker's [YouTube video](https://www.youtube.com/watch?v=9nogAYHmnNw) in 2020. The original vampire matrix is a square matrix $A$, usually $2 \times 2$ or $3\times 3$, with integer entries between $1$ and $9$ such that $A^2=11A$. I have worked on generalizing such matrices to include $d$ digit numbers and to include more terms in the matrix equation. A brief overview is given in a recent [conference presentation](/files/mccnny-2024.pdf) in March 2024. 