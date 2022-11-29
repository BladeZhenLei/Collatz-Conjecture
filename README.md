***
### Introduction
Probably considered one of the hardest and most famous unsolved problems in mathematics, sometimes called the $3X+1$ problem, it is named after mathematician Lothar Collatz, in 1937. The conjecture asks if given an odd number, the next term is 3 times the previous term plus 1, while given an even number, the next term is divided by 2. It is conjectured that these sequences will go on and always reach 1, no matter which positive integer is chosen to start the sequence.
The Collatz function can be defined as $T(n)=\frac{n}{2}$ if $n \equiv 0 \pmod{2}$, and $3n+1$ if $n\equiv 1 \pmod{2}$, we often denote the $k$-th iteration, that is, to apply the Collatz function $k$ times, as $T^{(k)}(n)$, and the Collatz sequence $C(n)=\lbrace n, T^{(1)}(n), T^{(2)}(n), T^{(3)}(n), ... , T^{(k)}(n) \rbrace$.
<p/>
The stopping time, $S(n)$, namely the number of steps to reach 1, is then the length of Collatz sequence minus 1, or $|C(n)|-1$, and the Collatz conjecture is stating that there exist a finite $k$ such that $T^{(k)}(n)=1$ for $n\geq2$, or in other words, $S(n)$ is finite.

### Irregular behaviour of S(N)

<p/><html lang="en"><head><meta http-equiv="content-type" content="text/html; charset=utf-8"><script type="text/javascript" charset="utf-8" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script></head>
