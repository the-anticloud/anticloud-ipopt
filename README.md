# IPOPT

> Anticloud offline package — upstream: coin-or/Ipopt @ `stable/3.14`.

## What This Project Does

COIN-OR Interior Point Optimizer IPOPT

## Upstream README

Ipopt
=====

Introduction
------------

Ipopt (Interior Point OPTimizer, pronounced eye-pea-Opt) is a software package for large-scale [nonlinear optimization](https://en.wikipedia.org/wiki/Nonlinear_programming).
It is designed to find (local) solutions of mathematical optimization problems of the form

$$\begin{align}
\min_{x \in R^n}\ & f(x), \\
\text{s.t.}\ & g_L \le g(x) \le g_U, \\
& x_L \le x \le x_U,
\end{align}$$

where $f: R^n \rightarrow R$ is the objective function, 
and $g: R^n \rightarrow R^m$ are the constraint functions.  The vectors $g_L$ and $g_U$ denote the lower and upper bounds on the constraints, and the vectors $x_L$ and $x_U$ are the bounds on the variables $x$.
The functions $f(x)$ and $g(x)$ can be nonlinear and nonconvex, but should be twice continuously differentiable.
Note that equality constraints can be formulated in the above formulation by setting the corresponding components of $g_L$ and $g_U$ to the same value.

Ipopt is part of the [COIN-OR Initiative](http://www.coin-or.org).
The Ipopt project webpage is <https://github.com/coin-or/Ipopt>.


Background
----------

Ipopt is written in C++ and is released as open source code under the [Eclipse Public License (EPL)](LICENSE).
The code has been written by [Andreas Wächter](http://www.mccormick.northwestern.edu/directory/profiles/Andreas-Waechter.html) and [Carl Laird](http://allthingsoptimal.com/biography/).
The COIN-OR project managers for Ipopt are [Andreas Wächter](http://users.iems.northwestern.edu/~andreasw) und [Stefan Vigerske](https://www.gams.com/~svigerske).
For a list of **all contributors**, see the [AUTHORS file](AUTHORS).

The C++ version has first been [released on Aug 26, 2005](http://list.coin-or.org/pipermail/ipopt/2005-August/000331.html) as version 3.0.0.
The previously released [pre-3.0 Fortran version](https://github.com/coin-or/Ipopt/tree/stable/2.3) is no longer maintained.


The Ipopt distribution can be used to generate a library that can be linked to one's own C++, C, Fortran, or Java code, as well as a solver executable for the [AMPL](http://www.ampl.com) modeling environment.
The package includes an interface to the [R](http://www.r-project.org/) programming environment.
IPOPT can be used on Linux/UNIX, macOS, and Windows platforms.

As open source software, the source code for Ipopt is provided without charge.
You are free to use it, also for commercial purposes.
You are also free to modify the source code (with the restriction that you need to make your changes public if you decide to distribute your version in any way, e.g. as an executable); for details see the EPL license.
And we are certainly very keen on feedback from users, including contributions!

In order to compile Ipopt, certain third party code is required (such as some linear algebra routines).
Those are available under different conditions/licenses.

If you want to learn more about Ipopt, you can find references in the [bibliography of the documentation](https://coin-or

## License

Upstream terms preserved in `THIRD_PARTY_LICENSES/`. Overlay licensed under Anticommons 0.1.0.

## Verification

Recompute the SHA3-256 of `BENCH.json` and compare to this package’s register. Any drift = invalid package.
