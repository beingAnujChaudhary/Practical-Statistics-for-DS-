# Practical Statistics for Data Scientists (2nd Edition)

A chapter-by-chapter Python implementation companion to *Practical Statistics for Data Scientists, 2nd Edition* by Peter Bruce, Andrew Bruce, and Peter Gedeck.

[![Python](https://img.shields.io/badge/Python-3.12%2B-blue)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

---

## Table of Contents

1. [Purpose](#purpose)
2. [Progress](#progress)
3. [Setup](#setup)
4. [Workflow](#workflow)
5. [Structure](#structure)
6. [References](#references)

---

## Purpose

This repository documents my chapter-by-chapter journey through *Practical Statistics for Data Scientists, 2nd Edition* using Python 3.12.10. It contains:

- From-scratch implementations of statistical concepts before using libraries
- Detailed chapter notes with key takeaways and formulas
- Exercises with hidden solutions for active recall practice
- Experimentation notebooks for exploring beyond the book
- Connections to real-world machine learning applications

**Focus:** Python-only implementation (R code from the book is ignored). All work is done in Google Colab and VS Code on Windows with PowerShell.

---

## Progress

| # | Chapter | Status |
|---|---------|:------:|
| 1 | Exploratory Data Analysis | ⬜ |
| 2 | Data and Sampling Distributions | ⬜ |
| 3 | Statistical Experiments and Significance Testing | ⬜ |
| 4 | Regression and Prediction | ⬜ |
| 5 | Classification | ⬜ |
| 6 | Statistical Machine Learning | ⬜ |
| 7 | Unsupervised Learning | ⬜ |

> ✅ = Completed | 🔄 = In Progress | ⬜ = Not Started

---

## Setup

### Prerequisites

- Python 3.12.10
- VS Code with Python and Jupyter extensions
- Git for Windows

### Local Setup (Windows + PowerShell)

```powershell
# 1. Clone the repository
git clone https://github.com/beingAnujChaudhary/Practical-Statistics-for-DS-.git
cd Practical-Statistics-for-DS-

# 2. Create and activate virtual environment
python -m venv venv
.\venv\Scripts\Activate.ps1

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open in VS Code
code .

# 5. Select venv kernel in VS Code: Ctrl+Shift+P → "Python: Select Interpreter"
```

### Google Colab (No Setup)

Open any notebook in the repository and click the "Open in Colab" badge, or upload directly to [Google Colab](https://colab.research.google.com). All dependencies are pre-installed.

---

## Workflow

Each chapter follows this learning sequence:

```
Read Chapter → Run Main Notebook → Complete Exercises → Explore in Experiments → Summarize in Notes → Commit
```

### Step-by-Step

1. **Read** the corresponding book chapter thoroughly
2. **Open** the main notebook (`0X_chapter_name.ipynb`)
3. **Run** all code examples cell by cell, modifying parameters to build intuition
4. **Complete** exercises in `exercises.ipynb` — attempt before viewing hidden solutions
5. **Experiment** in `experiments.ipynb` — break things, test edge cases, connect to ML concepts
6. **Document** key insights, formulas, and personal reflections in `chapter_notes.md`
7. **Commit** progress with descriptive messages

### Notebook Conventions

```python
# Standard imports for consistency
from utils.notebook_setup import *

# Fixed random seed for reproducibility
import numpy as np
np.random.seed(42)

# Data loading (use processed/ when available)
df = pd.read_csv('../datasets/processed/clean_data.csv')
```

---

## Structure

<details>
<summary>Click to expand repository structure</summary>

```
Practical-Statistics-for-DS/
│
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
├── datasets/
│   ├── raw/                    # Original data (never modified)
│   ├── processed/              # Cleaned, analysis-ready data
│   └── external/               # Third-party data
│
├── notes/                      # Cross-chapter reference notes
│   ├── statistics_cheatsheet.md
│   └── formulas.md
│
├── utils/                      # Reusable helper functions
│   ├── plotting.py
│   ├── stats_helpers.py
│   └── notebook_setup.py       # Common imports & configuration
│
├── chapter_01_exploratory_data_analysis/
│   ├── 01_exploratory_data_analysis.ipynb
│   ├── chapter_notes.md
│   ├── exercises.ipynb
│   ├── experiments.ipynb
│   ├── datasets/
│   └── output/
│
├── chapter_02_data_and_sampling_distributions/
│   ├── 02_data_and_sampling_distributions.ipynb
│   ├── chapter_notes.md
│   ├── exercises.ipynb
│   ├── experiments.ipynb
│   ├── datasets/
│   └── output/
│
├── chapter_03_statistical_experiments_and_significance_testing/
│   └── ...
│
├── chapter_04_regression_and_prediction/
│   └── ...
│
├── chapter_05_classification/
│   └── ...
│
├── chapter_06_statistical_machine_learning/
│   └── ...
│
└── chapter_07_unsupervised_learning/
    └── ...
```

</details>

### Chapter Contents

Each chapter folder contains four notebooks plus supporting files:

| File | Purpose |
|------|---------|
| `0X_chapter_name.ipynb` | Main implementation — book examples from scratch |
| `chapter_notes.md` | Key concepts, formulas, ML connections, personal reflections |
| `exercises.ipynb` | Practice problems with hidden solutions |
| `experiments.ipynb` | Personal explorations beyond the book |
| `datasets/` | Chapter-specific data files |
| `output/` | Generated plots and tables |

---

## Tech Stack

Core libraries used throughout (see `requirements.txt` for full list):

| Category | Libraries |
|----------|-----------|
| Data Manipulation | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn`, `plotly` |
| Statistics | `scipy`, `statsmodels` |
| Machine Learning | `scikit-learn` |
| Environment | `jupyter`, `notebook` |

---

## References

- [*Practical Statistics for Data Scientists, 2nd Edition*](https://www.oreilly.com/library/view/practical-statistics-for/9781492072935/) — Peter Bruce, Andrew Bruce, Peter Gedeck
- [Scipy Documentation](https://docs.scipy.org/doc/scipy/)
- [Statsmodels Documentation](https://www.statsmodels.org/stable/index.html)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)

---

## License

MIT License — See [LICENSE](LICENSE) for details.

> **Disclaimer:** This repository is for educational purposes only. All rights to the book content, examples, and datasets belong to the original authors and O'Reilly Media. Please purchase the book to support the authors.

