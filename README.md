# Computational Theory

This project implements the SHA-256 hashing algorithm step by step using Python and NumPy. The Jupyter notebook includes explanations, examples, and tests to demonstrate how the algorithm works. The project is currently in progress.

The work is in [`problems.ipynb`](problems.ipynb). It is still in progress.

## Progress

| Task | Status | Issue |
|---|---|---|
| Data representations | Complete | [#1](https://github.com/FawasAjani/computational-theory/issues/1) |
| SHA-256 bitwise operations | Complete | [#2](https://github.com/FawasAjani/computational-theory/issues/2) |
| Generating SHA-256 constants | Complete | [#3](https://github.com/FawasAjani/computational-theory/issues/3) |
| Padding and parsing messages | In progress | [#4](https://github.com/FawasAjani/computational-theory/issues/4) |
| Compression function | Not started | [#5](https://github.com/FawasAjani/computational-theory/issues/5) |
| Full SHA-256 implementation | Not started | [#6](https://github.com/FawasAjani/computational-theory/issues/6) |

## How to Run

Install [Python](https://www.python.org/) and [Git](https://git-scm.com/), then run the following commands in your terminal:

```bash
git clone https://github.com/FawasAjani/computational-theory.git
cd computational-theory
python -m pip install -r requirements.txt
jupyter notebook problems.ipynb
```

In Jupyter Notebook, run the cells from top to bottom.

## Dependencies

- NumPy
- Jupyter Notebook
- ipykernel