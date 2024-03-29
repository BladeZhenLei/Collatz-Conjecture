<h3>Introduction</h3>
Probably the hardest unsolved problems in mathematics, also called the $3X+1$ problem, it is named after the mathematician Lothar Collatz in 1937. The conjecture asks if given an odd number, the next term is 3 times the previous term plus 1, while given an even number, the next term is divided by 2. It is conjectured that these sequences will go on and always reach 1, no matter which positive integer is chosen to start the sequence.
<p/>
The Collatz function can be defined as $T(n)=\frac{n}{2}$ if $n \equiv 0 \pmod{2}$, and $3n+1$ if $n\equiv 1 \pmod{2}$. We often denote the $k$-th iteration, that is to apply the Collatz function $k$ times, as $T^{(k)}(n)$, and the Collatz sequence is $C(n)=\lbrace n, T^{(1)}(n), T^{(2)}(n), T^{(3)}(n), ... , T^{(k)}(n) \rbrace$.
<p/>
Then the stopping time $S(n)$ is said to be the length of $C(n)$ minus 1, and the Collatz conjecture asserts that $S(n)$ is finite for all $n\geq{2}$. For Example, $C(3)=\lbrace 3, 10, 5, 16, 8, 4, 2, 1 \rbrace$, and $S(3)=|C(3)|-1=7$.  Plot below shows $S(n)$ for $1\leq{n}\leq{10000}$.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/205472558-b2fabe57-7635-4ab1-b0ca-e4ae3d20c849.png" width="500" height="350"> <p/>


<h3>The Irregular behaviour of $S(n)$</h3>
Interestingly, it seems like there is almost a logarithmic pattern, but not quite...by switching to the $log(x)-y$ plot, the dots are aligned on some lattices, however, shifted aways.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/205472604-ce2e8c30-79be-4f58-8515-69658587755a.png" width="500" height="350"> <p/>
If we define $E(n)$ as the even terms and $O(n)$ as the odd terms in $C(n)$, then some explicit relationships can be observed.
<br/>
First, we have a trivial expansion 
$$S(n)=|E(n)|+|O(n)|=log_2(6^{|O(n)|}\cdot{n})+log_2(\frac{2^{|E(n)|}}{n\cdot{3^{|O(n)|}}}),$$
then, let
$$\epsilon(n)=\frac{2^{|E(n)|}}{n\cdot{3^{|O(n)|}}}=\prod_{q\,\in\,{O(n)}}\frac{3q+1}{3q},$$
this error term can be interpreted as a product over all odd terms.
It is computer verified that for all $n\leq{10^7}$, there is
$$\epsilon(n)\leq\epsilon(993)=2305843009213693952/1840049047529878113,$$
and $\epsilon(n)$ is called the 'residue' of the sequence. 
<p/>
Heuristic studies highly suggests that $\epsilon(993)=\epsilon(993\cdot{2^k})\approx1.25314$ is the absolute upper bound for all Collatz sequence, as far as the conjecture holds true.
<p/>

<h3>Finiteness of Stopping Time</h3>
In 1976 Riho Terras made an important advancement in this problem, stating that the fraction of numbers that do not have finite stopping time is approaching $0$ as $n\rightarrow{\infty}$. This is called the Terras Theorem, where it shows 'almost all' Collatz sequences are convergent. This approach was further improved by Terence Tao in 2019.
<p/>
Basically, if one can prove that non-trivial cycle in fact does not exist, then this would prove a weaker version of the Collatz Conjecture. Eliahou (1993) used a diffrent method based on Diophatine approximation of $log(3)/log(2)$, where its expansion has Farey sequences satisfying a lower bound of 17087915 for a non-trivial Collatz cycle to exist.

<h3>Mystery Unsovled</h3>
Several generalized versions of Collatz Conjecture have been proven to be 'undecidable', i.e., Conway (1972), meaning that our modern mathematics is completely useless as to provide a yes-or-no answer to such problems. However, it is not yet identified whether the original $3X+1$ problem is decidable.
<p/>


<p/><html lang="en"><head><meta http-equiv="content-type" content="text/html; charset=utf-8"><script type="text/javascript" charset="utf-8" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script></head>

