### Main Conjectures
There are two simple and common ways of constructing computable large numbers, one is through repeated exponentials (tertration), and the other one is through stacked factorials (multifactorials), both do not involve complicated arithmetical hierachy. But still, many of these numbers have magnitude that are well beyond the capacity of conventional computers, it can only be hoped that advances in additive number theory or quantum computers can help further understand their related problems. All of the following conjectures/problems are originally created by me, some are inspired by others.
<p/>

**1. Tower of $2$ and $3$ Sum (2022.1.19; solved)**
<br/>
Denote the tetration of an integer $a$ as ${^{n}a}=a^{a^{a^{.^{.^{.}}}}}$ where the exponent is repeated $n$ times. Other than $p_1$, $p_2$, and $p_3$, are there more primes in the form $p_n={^{n}2}+{^{n}3}=3^{3^{3^{.^{.^{.}}}}}+2^{2^{2^{.^{.^{.}}}}}$?
<br/>
<strong> Answer </strong>
<p/>
[Note: It is impossible to calculate $p_4$ itself, as it is several magnitudes bigger (3,638,334,640,024 digits) than the largest prime number that human ever computed (24,862,048 digits), the first result was obtained using trial division method through exhaustive cloud computing, it took more than a month to find the smallest divisor, which should be credited to the original author. The second incredible general case result was obtained by another author under the same post using Extended Euler's Theorem. See <a href="https://www.zhihu.com/question/512482114/answer/2319816820?utm_id=0"> Is 2^2^2^2+3^3^3^3 prime? (In Chinese) </a>.]
<p/>
No, the frist three terms are the only primes in such pattern.
<br/>
For $n=4$, we have $21219553216129$ divides $p_4$.
<br/>
For $n>{4}$, we have $34276387$ divides $p_5$, and in general, $4423$ divides $p_6$ or greater.
<br/>
<strong> $Proof.$ </strong>
<br/>
The case for $p_4$ can be shown as follow: $3^{3^{3^{3}}}={(3^{3^{20}})}^{2187}=2210105334066^{2187} \equiv 212195553150593 &ensp; (mod &ensp; 21219553216129),3^{3^{3^{3}}}+2^{2^{2^{2}}}=65536+21219553150593\equiv{0 &ensp;(mod&ensp; 21219553216129)}.$
Let $\phi^{k}(n)$ be the $k$ layers of the $Euler$ function, then there exist $n>m$ such that $\phi^{m}(n)=1$. For $x={^{b}a}&ensp;(mod&ensp;n)$, if we find $b>l>m$ such that ${^{l-m}a}>n$, then $x$ is constant. 
<br/>
For example, we have $\phi^{11}(4423)=1$, ${^{5}2}>4423$, then ${^{b}2}&ensp;(mod&ensp;4423)=2197$, and ${^{b}3}&ensp;(mod&ensp;4423)=2226$, therefore ${^{b}2}+{^{b}3}=2197+2226&ensp;(mod&ensp;4423)=0&ensp;(mod&ensp;4423).$  


**[Generalized] $2$-Tower Sum (2023.2.13; open)**
<br/>
How many primes are there in the form of ${^{n}a}+{^{n}b}$, finitely or infinitely many?
<br/>
<strong> Comment </strong>
<br/>
None.

**[Generalized] $N$-Tower Sum (2023.2.13; open)**
<br/>
How many prime divisors are there for all such ${^{e_1}1}+{^{e_2}2}+...+{^{e_n}n}$, where $e_{i+1}>e_{i}$, could there be only finitely many?
<br/>
<strong> Comment </strong>
<br/>
None.

**2. $N$-Factorial Sum (2022.10.9; open)** 
<br/>
For any integer $n\geq{1}$, is there always a prime that can be obtained from combinations of addition and subtraction of all elements in the set $\lbrace{1!, 2!, 3!, …, n!}\rbrace$? 
Such as
$p_1={1!}\pm{0!},$
$p_2={2!}\pm{1!},$
$p_3={3!}\pm{2!}\pm{1!},$
$\cdots,$
$p_n=n!\pm(n-1)!\pm(n-2)!\pm(n-3)!\pm\cdot\cdot\cdot\pm{1!}.$
<br/>
<strong> Comment </strong>
<br/>
This statement reamins true for $p_{1}$ to $p_{257}$ and likely to be true for all positive integers. Considering the prime density around $n!$ with such combination shoud be $\frac{2^{n-1}}{nlog(n)}>1$.

**[Specified] $2$-Factorial Sum (2022.10.10; open)**
<br/>
For any given $n\in{N}$, let $k\in{Z}$ such that $n\geq{k}\geq{1}$, define $S=\lbrace{n!}\pm{k!}\pm{1}\rbrace\cap{P}$, is $S^c$ a finite set?
<br/>
<strong> Comment </strong>
<br/>
The known examples are only $n=\lbrace{63, 161, 382, 902}\rbrace$ for $n\leq1250$.

**3. $N$-Collatz Sum (2022.10.25; open)**
<br/>
If we assign $\pm$ to all elements of a Collatz sequence, i.e.
$S(1)=1$,
$S(2)=2-1$,
$S(3)=3-10+5+16-8-4-2+1$,
$S(4)=4-2-1$,
$S(5)=5-16+8+4-2+1$, ...,
is it true that $\min(|S(n)|)\leq{1}$ always hold?  
<strong> Comment </strong>
<br/>
This is verified to be true for $n\leq{10^6}$.



### Computation Problems
**1.** Is $2\cdot3^{3^{3^{3}}}-1$ prime?
<br/>
<strong> Answer </strong>
<br/>
No, it has the smallest non-trivial divisor $2504371752217$.

**2.** Is $3^{3^{3^{3}}}+4$ prime?
<br/>
<strong> Comment </strong>
<br/>
None.

**3.** Is $3^{3^{2^{2^{2}}}}-2^{2^{2^{2^{2}}}}$ prime?
<br/>
<strong> Comment </strong>
<br/>
None.


<p/>
<html lang="en">
<head>
<meta http-equiv="content-type" content="text/html; charset=utf-8">
<script type="text/javascript" charset="utf-8" src="
https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>
