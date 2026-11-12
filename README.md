# SHA-256 Implementation

This project implements the SHA-256 hashing algorithm step by step using Python and NumPy. The Jupyter notebook explains each part of the algorithm and includes code examples and tests. The final `sha256(msg)` function matches Python's `hashlib.sha256` on every test input. `hashlib` is used only to check my results, never to compute them.

## Table of Contents

- [Progress](#progress)
- [What the Notebook Covers](#what-the-notebook-covers)
- [Repository Structure](#repository-structure)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [Use of AI](#use-of-ai)
- [References](#references)

## Progress

| Task | Status | Issue |
|---|---|---|
| Problem 1: Representing SHA-256 Data | Complete | [#1](https://github.com/FawasAjani/computational-theory/issues/1) |
| Problem 2: SHA-256 Bitwise Operations | Complete | [#2](https://github.com/FawasAjani/computational-theory/issues/2) |
| Problem 3: Generating SHA-256 Constants | Complete | [#3](https://github.com/FawasAjani/computational-theory/issues/3) |
| Problem 4: Padding and Parsing Messages | Complete | [#4](https://github.com/FawasAjani/computational-theory/issues/4) |
| Problem 5: Compression Function | Complete | [#5](https://github.com/FawasAjani/computational-theory/issues/5) |
| Problem 6: Full SHA-256 Implementation | Complete | [#6](https://github.com/FawasAjani/computational-theory/issues/6) |

The code and explanations for each problem are in [`problems.ipynb`](problems.ipynb).

## What the Notebook Covers

1. **Data representation:** how words, blocks, messages and the hash are stored in Python.
2. **Bitwise functions:** `Ch`, `Maj`, `Sigma0`, `Sigma1`, `sigma0` and `sigma1` on 32-bit unsigned integers.
3. **Constants:** the 64 round constants, generated from prime roots and checked against the standard.
4. **Padding and parsing:** the `block_parse` generator, tested around the 55, 56 and 64-byte boundaries.
5. **Compression function:** the 64-word message schedule and the 64 rounds.
6. **Complete `sha256(msg)`:** tested against `hashlib` on empty, ASCII, non-ASCII, boundary-length and long messages.

The whole notebook runs in a few seconds.

## Repository Structure

```text
computational-theory/
├── README.md
├── problems.ipynb
├── requirements.txt
├── .gitignore
└── AGENTS.md
```

The project needs no data files or images, so there are no `data/` or `img/` folders.

## How to Run

### Requirements

- Python 3.10 or later (tested on 3.10.9)
- Git

### 1. Clone the repository

Open a terminal and run:

```bash
git clone https://github.com/FawasAjani/computational-theory.git
cd computational-theory
```

### 2. Install the dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook problems.ipynb
```

Run the cells from top to bottom using **Shift + Enter**, or select **Run All** from the notebook menu.

## Dependencies

Listed in `requirements.txt`:

- **NumPy:** used for numerical operations and 32-bit unsigned integers.
- **Jupyter Notebook:** used to open and run the notebook.
- **ipykernel:** provides the Python kernel used to execute notebook cells.

## Use of AI

I wrote the original code, comments and explanations myself. I used Claude (Anthropic) to draft docstrings, test cases, some explanations and formulas. I applied and checked everything myself against Python's `hashlib`.

## References

- **NIST, [FIPS 180-4: Secure Hash Standard](https://doi.org/10.6028/NIST.FIPS.180-4).** Main reference for the SHA-256 algorithm, including its bitwise operations, padding rules, and round constants.
- **Eastlake, D. 3rd and Hansen, T., [RFC 6234: US Secure Hash Algorithms (SHA and SHA-based HMAC and HKDF)](https://www.rfc-editor.org/rfc/rfc6234), 2011.** A second description of the algorithm with a reference implementation in C, used for comparison.
- **[Merkle–Damgård construction](https://en.wikipedia.org/wiki/Merkle–Damgård_construction), Wikipedia (accessed 10 November 2026).** Background on the construction that SHA-256 follows.
- **[NumPy documentation](https://numpy.org/doc/stable/).** Reference for NumPy data types and numerical functions.
- **[Python documentation](https://docs.python.org/3/).** Reference for Python and its standard library, including `hashlib` for testing the completed hash implementation.

---

**Author:** Fawas Ajani