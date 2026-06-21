# Code and Data

This repository provides the code and data associated with the preprint ***Algebraic structure of the smallest degenerate zero-one reaction networks*** by Xiaoxian Tang and Yuanlin Chen. Preprint link: https://xxx.

## Computational Verification

Case (2) of Lemma 3.16 can be verified using the Mathematica script `code1.nb`. The associated data file `35-m.txt` contains the (m)-column submatrices of matrix (35) in which at least one column vector belongs to ({(-1,-1),(1,1)}), together with the corresponding reactant matrices.

Lemma 3.17 can be verified using the Mathematica script `code2.nb`. The associated data file `36-m.txt` contains the (m)-column submatrices of matrix (36) in which at least one column vector belongs to ({(-1,1),(1,-1)}), together with the corresponding reactant matrices.

## Data Format

Each row of the data file consists of a pair ({N,X}), where (N) is the stoichiometric matrix and (X) is the reactant matrix. For example, the first row in `35-4.txt` is

[
\left{
\left{{-1,1,-1,-1},{-1,1,0,0}\right},
\left{{1,1},{0,0},{1,0},{1,1}\right}
\right}.
]

Here,

[
N=
\begin{pmatrix}
-1 & 1 & -1 & -1 \
-1 & 1 & 0 & 0
\end{pmatrix},
\qquad
X=
\begin{pmatrix}
1 & 0 & 1 & 1 \
1 & 0 & 0 & 1
\end{pmatrix}.
]

With species (X_1) and (X_2), the corresponding reaction network is

[
X_1+X_2 \xrightarrow{\kappa_1} 0,\quad
0 \xrightarrow{\kappa_2} X_1+X_2,\quad
X_1 \xrightarrow{\kappa_3} 0,\quad
X_1+X_2 \xrightarrow{\kappa_4} X_2.
]
