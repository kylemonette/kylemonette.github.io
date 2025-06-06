---
title: 'Vampire Matrices'
date: 2025-6-6
permalink: /posts/2025/6/vampire-matrices/
tags:
  - Vampire Matrices
---


On Halloween in 2020, Matt Parker of the YouTube Channel *Standup Maths* posted a [video](https://www.youtube.com/watch?v=9nogAYHmnNw) about *Vampire Matrices*. In this early definition of the term, Parker defined a (single) Vampire Matrix to be a square matrix consisting of positive integers such that the square of the matrix is equal to its element-wise concatenation.
As a $2\times 2$ example,
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
\\] As Parker illustrates in his video, himself and other mathematicians on YouTube and Twitter noticed that these matrices satisfy the equation
\\begin{equation}\label{eq1}
A^2 = 11 A
.\\end{equation}
If we allow for two-digit integer entries (by this I mean *strictly* two-digit numbers to rule out things like $04$ which is really just $4$, a one-digit number), then the matrix equation of interest becomes
\\begin{equation}\label{eq2}
A^2 = 101 A
.\\end{equation} One such matrix is
\\[
\mat{cc}
60 & 30 \\\\ 82 & 41 \rix^2 = \mat{cc} 6060 & 3030 \\\\ 8282 & 4141 \rix.
\\]

Can we have a *pair of matrices* for which their product is equal to their element-wise concatenation? Yes! For example,
\\[
\mat{cc} 4 & 8 \\\\ 2 & 3 \rix \mat{cc} 8 & 8 \\\\ 2 & 7 \rix = \mat{cc} 48 & 88 \\\\ 22 & 37 \rix.
\\]
Here entries are one-digit integers and so the corresponding matrix equation is
\\begin{equation}\label{eq3}
AB = 10A + B.
\\end{equation}

Now, we start to see the pattern. Equation \eqref{eq3} reduces to \eqref{eq1} if $A=B$. And in the last example if we had strictly two-digit integers in the matrices on the left-hand side, then \eqref{eq3} would be $AB = 100A + B$ and then becomes \eqref{eq2} in the special case when $A=B$.

To clarify some things and make this development more rigorous, let's define some terms.

<ul>
<li>Let $N_d = \{n \in \mathbb{N} \mid n \text{ has exactly } d \text{ digits}\}$.</li>
  <ul>
  <li>For example, $N_1 = \{ 1, \dots, 9\}$ and $N_2 = \{10, \dots, 99\}$.</li>
  </ul>
<li>Let $N_d^{n \times n}$ be the set of $n\times n$ matrices with entries in $N_d$.</li>
<li>A set of matrices $\{A_1, \dots, A_k\}$ in $N_d^{n \times n}$ is said to satisfy the <em>multiplication concatenation property</em> (MCP) if
$\prod_{i=1}^k A_i \; = \; \sum_{i=1}^k 10^{d(k-i)} A_i$.</li>
</ul>

We have proven some elementary properties so far about matrices $A \in N_d^{n\times n}$ which satisfy the MCP <em>by themselves</em>. That is, the set of matrices is $\{A,A\}$ and so $A^2 = (10^d+1)A$.
<ol>
<li>Eigenvalues of $A$ are $0$ and $10^d+1$, with multiplicities $n-1$ and $1$, respectively. This means the trace of $A$ is $10^d+1$.</li>
<li>Therefore, $A$ is singular. In fact, for these matrices to satisfy the MCP it is sufficient and necessary that $A$ is singular and has trace $10^d+1$. <em>In the case of two or more matrices satisfying the MCP, this biconditional statement is no longer true.</em></li>
</ol>

This project is a work in progress, and I welcome anyone interested in "joining it" to reach out to me! Here are some ideas I have on what to pursue:
<ol>
<li>Is there a size limit on the matrices for which $A^2 = (10^d+1)A$? We have found examples of size $n=2, 3, 4$.</li>
<li>Can we think about solving the matrix equation in the MCP? That is, can we generate them in some manner?</li>
<li>Are there matrices $B$ so that $\mathcal{A} = \{ A_1, \dots, A_k\}$ satisfies the MCP but $\mathcal{A} \cup B$ does not?</li>
</ol>