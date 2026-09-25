# Numerical Verification of the Residue Theorem

This project contains a computational study of the residue theorem for

$$f(z)=\frac{1}{z^2+1}.$$

The notebook compares contour integrals evaluated numerically from an explicit
parameterization with the corresponding values obtained from residues. These
experiments provide numerical verification of the theorem's predictions; they
are not a proof of the residue theorem.

## Experiments

The executed notebook studies five contours, with no pole placed on a contour:

1. A counterclockwise circle containing no poles.
2. A counterclockwise circle containing one pole.
3. A counterclockwise circle containing both poles.
4. A clockwise traversal of a circle containing one pole.
5. Two counterclockwise traversals of a circle containing one pole.

The corresponding results are $0$, $\pi$, $0$, $-\pi$, and $2\pi$.
For the case containing both poles, the residues cancel:

Res(f, i) = 1/(2i) = −i/2; Res(f, −i) = −1/(2i) = i/2. Their sum is zero.

The maximum absolute error in the executed table is
`4.456537e-16`.

## Files

- [`residue_experiments.ipynb`](residue_experiments.ipynb) — executed notebook with numerical results and contour plots.
- [`Untitled-1.ipynb`](Untitled-1.ipynb) — original notebook retained unchanged.



## Assignment and AI Assistance


This project numerically investigates the residue theorem using Python. AI assistance was used to help organize the notebook, implement the numerical
experiments, and check the reported results. This is a work in progress. I am
reviewing the mathematical reasoning and interpretation alongside the
computational checks.

## Next Stage

The next stage will investigate numerical accuracy as the contour approaches a
pole. This experiment has not yet been performed.
