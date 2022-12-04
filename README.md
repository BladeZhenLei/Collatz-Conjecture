***
<h3>Introduction</h3>
Probably considered one of the hardest and notorious unsolved problems in mathematics, sometimes called the $3X+1$ problem, it is named after mathematician Lothar Collatz, in 1937. The conjecture asks if given an odd number, the next term is 3 times the previous term plus 1, while given an even number, the next term is divided by 2. It is conjectured that these sequences will go on and always reach 1, no matter which positive integer is chosen to start the sequence.
The Collatz function can be defined as $T(n)=\frac{n}{2}$ if $n \equiv 0 \pmod{2}$, and $3n+1$ if $n\equiv 1 \pmod{2}$, we often denote the $k$-th iteration, that is, to apply the Collatz function $k$ times, as $T^{(k)}(n)$, and the Collatz sequence $C(n)=\lbrace n, T^{(1)}(n), T^{(2)}(n), T^{(3)}(n), ... , T^{(k)}(n) \rbrace$.
<p/>
Then the stopping time $S(n)$ is said to be the length of $C(n)$ minus 1, and the Collatz conjecture asserts that all $S(n)$ is finite for all $n\geq{2}$.
<p/>
Below is a plot of $S(n)$ for $1\leq{n}\leq{10000}$.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/205472558-b2fabe57-7635-4ab1-b0ca-e4ae3d20c849.png" width="500" height="350"> <p/>


<h3>The Irregular behaviour of $S(N)$</h3>
It seems like there is almost a logarithmic pattern in there, but not quite...by switching to the log-log plot, the dots are almost aligned on some lattices, however, shifting aways.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/205472530-2c6695b8-3615-4476-b01f-8d970394184a.png" width="500" height="350"> <p/>


<p/><html lang="en"><head><meta http-equiv="content-type" content="text/html; charset=utf-8"><script type="text/javascript" charset="utf-8" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script></head>
