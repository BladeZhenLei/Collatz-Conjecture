***
<h3>Introduction</h3>
Probably considered one of the hardest and notorious unsolved problems in mathematics, sometimes called the $3X+1$ problem, it is named after mathematician Lothar Collatz, in 1937. The conjecture asks if given an odd number, the next term is 3 times the previous term plus 1, while given an even number, the next term is divided by 2. It is conjectured that these sequences will go on and always reach 1, no matter which positive integer is chosen to start the sequence.
The Collatz function can be defined as $T(n)=\frac{n}{2}$ if $n \equiv 0 \pmod{2}$, and $3n+1$ if $n\equiv 1 \pmod{2}$, we often denote the $k$-th iteration, that is, to apply the Collatz function $k$ times, as $T^{(k)}(n)$, and the Collatz sequence $C(n)=\lbrace n, T^{(1)}(n), T^{(2)}(n), T^{(3)}(n), ... , T^{(k)}(n) \rbrace$.
<p/>
Then the stopping time $S(n)$ is said to be the length of $C(n)$ minus 1, and the Collatz conjecture asserts that all $S(n)$ is finite for all $n\geq{2}$.
<p/>
Below is a plot of $S(n)$ for $1\leq{n}\leq{10000}$.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/204690527-18770b2f-e51b-4647-98f8-753be28f24db.png" width="500" height="400"> <p/>

<h3>The Irregular behaviour of $S(N)$</h3>
<p/><html lang="en"><head><meta http-equiv="content-type" content="text/html; charset=utf-8"><script type="text/javascript" charset="utf-8" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script></head>
