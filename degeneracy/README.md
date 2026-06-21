# Code and Data

This repository provides the code and data associated with the preprint
***Algebraic structure of the smallest degenerate zero-one reaction networks***
by Xiaoxian Tang and Yuanlin Chen.

Preprint link: https://xxx

---

## Computational Verification of Lemma 3.16

Case (2) of Lemma 3.16 can be computationally verified using the Mathematica script

```text
code1.nb
```

The associated data files

```text
35-m.txt
```

contain the (m)-column submatrices of matrix (35) in which at least one column vector belongs to
[
{(-1,-1),(1,1)},
]
together with the corresponding reactant matrices.

---

## Computational Verification of Lemma 3.17

Lemma 3.17 can be computationally verified using the Mathematica script

```text
code2.nb
```

The associated data files

```text
36-m.txt
```

contain the (m)-column submatrices of matrix (36) in which at least one column vector belongs to
[
{(-1,1),(1,-1)},
]
together with the corresponding reactant matrices.

---

## Interpreting the Data

We illustrate how to convert the provided data into reactions. For example, the first row in `35-4.txt` is

[
\left{
\left{
{-1,1,-1,-1},{-1,1,0,0}
\right},
\left{
{1,1},{0,0},{1,0},{1,1}
\right}
\right}.
]

Let the species be denoted by (X_1) and (X_2).

The first element

[
\left{
{-1,1,-1,-1},{-1,1,0,0}
\right}
]

represents the stoichiometric matrix

[
N=
\begin{pmatrix}
-1 & 1 & -1 & -1 \
-1 & 1 & 0 & 0
\end{pmatrix}.
]

The second element

[
\left{
{1,1},{0,0},{1,0},{1,1}
\right}
]

represents the reactant matrix

[
Y=
\begin{pmatrix}
1 & 0 & 1 & 1 \
1 & 0 & 0 & 1
\end{pmatrix}.
]

Thus, the corresponding reaction network is

[
X_1+X_2 \xrightarrow{\kappa_1} 0,\qquad
0 \xrightarrow{\kappa_2} X_1+X_2,\qquad
X_1 \xrightarrow{\kappa_3} 0,\qquad
X_1+X_2 \xrightarrow{\kappa_4} X_2.
]
