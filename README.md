# Mirror Wave Function of Prime Numbers

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository accompanies the paper  
**"The Mirror Wave Function of Prime Numbers: An Unexpected Discovery"**  
(Revised and corrected version, July 31, 2025).

## Overview

We study the **Discrete Fourier Transform (DFT)** of the modular wave function:

\[
\psi_p(x) = \chi(p)\, e^{i\frac{2\pi}{q} p^{-1} x},
\]

where \(q \ge 2\), \(\chi\) is a primitive Dirichlet character modulo \(q\), and \(p\) is coprime to \(q\).  
Our main theorem states that the DFT of \(\psi_p\) is a **perfect Kronecker delta peak**:

\[
\widehat{\psi}_p(k) =
\begin{cases}
\chi(p)\sqrt{q}, & k \equiv p^{-1} \pmod q,\\
0, & \text{otherwise}.
\end{cases}
\]

This reveals a direct spectral signature of modular inverses, with potential applications in number theory and signal processing.

All formal proofs, definitions, and numerical examples are provided in the **full PDF paper** (see [`paper/`](paper/)).

## Repository Content

- [`paper/`](paper/) – Contains the PDF version of the article (and LaTeX source if available).
- [`code/`](code/) – Python scripts to compute and plot the DFT for the examples in the paper.
- [`figures/`](figures/) – Generated plots showing the spectral peaks for \(q=5, p=2\) and \(q=13, p=7\).

## Getting Started

### Prerequisites

- Python 3.6+
- NumPy
- Matplotlib

Install dependencies with:

```bash
pip install -r code/requirements.txt
