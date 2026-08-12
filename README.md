# Jaccard Needs Exponentially Many Convex Scores

## Abstract

Jaccard similarity, also called intersection over union, and the F1 score are pointwise monotone transforms of one another. Their convex surrogate complexities are nevertheless exponentially different. For instance-wise multi-label prediction with $s$ labels, we prove 

$$2^{s-1}-1 \\,\leq\\, \mathrm{CCdim}(L^{\rm Jac}) \\,\leq\\, 2^s-1.$$

 Thus every convex surrogate calibrated for Jaccard on all conditional label distributions needs exponentially many real-valued scores. In contrast, a recent tight result gives convex calibration dimension $\Theta(s^2)$ for F1. The lower bound comes from one explicit conditional distribution. It is supported on all sets containing a fixed core label, weights a set with $d$ optional labels by $1/d!$, and makes exactly those $2^{s-1}$ reports Bayes optimal. Strict positive definiteness of the corresponding Jaccard block then collapses its feasible Bayes subspace to a point. We also identify an algebraic phase transition. In the normalized-overlap family interpolating from Dice/F1 to Jaccard, the exact score-matrix rank is $s^2-s+2$ at the F1 endpoint but $2^s$ after any positive Jaccard correction. Finally, we reconcile our theorem with a NeurIPS 2024 claim that an $s$-score convex logistic surrogate is Bayes-consistent for every multi-label loss. A two-label rational example gives zero surrogate regret and Jaccard regret $1/10$. The proof in that work transfers probability between two arbitrary label vectors, but its additive softmax probabilities form only an $s$-dimensional product family and cannot realize that transfer. Our results separate practical restricted-distribution methods from distribution-free convex calibration and show that, for Jaccard, this distinction is unavoidable.

## Contributions

- We prove an exponential lower bound
$\mathrm{CCdim}(L^{\rm Jac})\geq 2^{s-1}-1$. The standard affine upper bound is
$2^s-1$, determining the order exactly.
- We give an explicit factorially weighted Bayes witness and a short
combinatorial identity showing that precisely all reports containing one
core label tie. This produces exponentially many independent active Bayes
constraints at one distribution.
- We prove a sharp rank discontinuity for a continuous family of
normalized-overlap scores. The F1 endpoint has quadratic rank, while every
positive Jaccard correction has full rank $2^s$.
- We give a rational two-label falsification certificate for the claimed
general consistency of the low-dimensional multi-label logistic loss. It
has zero surrogate regret but positive target regret, and does not depend on
the empty-set convention.

## Keywords

convex calibration dimension, Jaccard index, intersection over union, surrogate losses, multi-label prediction, lower bounds

## Files

- `main.pdf`
- `main.tex`
- `references.bib`
- `iclr2027_conference.sty`, `iclr2027_conference.bst`, `natbib.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
