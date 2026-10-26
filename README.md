# SHA-256 Implementation

This project implements the SHA-256 hashing algorithm step by step using Python and NumPy. The Jupyter notebook explains the different parts of the algorithm and includes code examples and tests.

## Table of Contents

- [Progress](#progress)
- [Repository Structure](#repository-structure)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [References](#references)

## Progress

| Task | Status | Issue |
|---|---|---|
| Problem 1: Representing SHA-256 Data | Complete | [#1](https://github.com/FawasAjani/computational-theory/issues/1) |
| Problem 2: SHA-256 Bitwise Operations | Complete | [#2](https://github.com/FawasAjani/computational-theory/issues/2) |
| Problem 3: Generating SHA-256 Constants | Complete | [#3](https://github.com/FawasAjani/computational-theory/issues/3) |
| Problem 4: Padding and Parsing Messages | Complete | [#4](https://github.com/FawasAjani/computational-theory/issues/4) |
| Problem 5: Compression Function | Not started | [#5](https://github.com/FawasAjani/computational-theory/issues/5) |
| Problem 6: Full SHA-256 Implementation | Not started | [#6](https://github.com/FawasAjani/computational-theory/issues/6) |

The code and explanations for each problem are in [`problems.ipynb`](problems.ipynb).

## Repository Structure

```text
computational-theory/
├── README.md
├── problems.ipynb
├── requirements.txt
├── .gitignore
└── AGENTS.md
```

## How to Run

### Requirements

- Python 3
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

- **NumPy** — used for numerical operations and 32-bit unsigned integers.
- **Jupyter Notebook** — used to open and run the notebook.
- **ipykernel** — provides the Python kernel used to execute notebook cells.

## References

- **NIST, FIPS 180-4: Secure Hash Standard.** [Official publication](https://doi.org/10.6028/NIST.FIPS.180-4). Reference for the SHA-256 algorithm, including its bitwise operations, padding rules, and round constants.
- **NumPy documentation.** [Official documentation](https://numpy.org/doc/stable/). Reference for NumPy data types and numerical functions.
- **Python documentation.** [Official documentation](https://docs.python.org/3/). Reference for Python and its standard library, including `hashlib` for testing the completed hash implementation.

---

**Author:** Fawas Ajani