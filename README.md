# ExtrBettiNumbers
A CoCoA package for compute graded ideals of a polynomial ring with given extremal Betti numbers. Please find more details about the package in this [paper](https://www.sciencedirect.com/science/article/pii/S0747717118300506).

Introduction
===================
The algorithms implemented in the package `ExtrBettiNumbers` are devoted to easy compute graded ideals of this ring with given extremal Betti numbers (positions as well as values).

The package contains two public functions:
- The function `StronglyStableIdealEB($R$, Corners, $a$, print)'` requires as input parameters a polynomial ring ($R$), a corner sequence (Corners), a corner values sequence ($a$), and a boolean value to control the printing. It determines the conditions under which, given two positive integers $n, r$, $1\le r \le n-1$, there exists a graded ideal of a polynomial ring $R$ in $n$ variables with $r$ extremal Betti numbers $a$ in the given corners. In the case of a positive answer, it returns the minimal set of monomial generators of the Finitely Generated Borel Ideal we are looking for. 
- The function `AdmissibleValues($R$, Corners)` requires as input parameters a polynomial ring ($R$), and a corner sequence (Corners). It checks whether an $r$-tuple of positive integers represents the admissible values of the $r$ extremal Betti numbers in the given corners. As a result, the procedure returns a table whose columns are the admissible $r$-tuple $a=(a_1, \ldots, a_r)$ in the given corners, i.e., the configurations of extremal Betti numbers (positions as well as values) for which the Finitely Generated Borel Ideal exists.
