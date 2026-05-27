# Practical Statistics for Data Scientists (3rd Edition) — Python Implementation

> 📘 **A companion repository for working through *"Practical Statistics for Data Scientists, 3rd Edition"* by Peter Bruce, Andrew Bruce, and Peter Gedeck — strictly implemented in Python.**

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

---

## 📑 Table of Contents
1. [🎯 Project Goal](#-project-goal)
2. [📚 Chapter Progress](#-chapter-progress)
3. [🚀 Quick Start Guide](#-quick-start-guide)
4. [🧰 Tools & Libraries](#-tools--libraries)
5. [📝 Repository Workflow](#-repository-workflow)
6. [🗂️ Data Management](#-data-management)
7. [📂 Directory Structure](#-directory-structure)

---

## 🎯 Project Goal

The objective of this repository is to work through *Practical Statistics for Data Scientists* chapter-by-chapter, translating and implementing all statistical concepts, examples, and exercises into **Python**. 

**Environment & Workflow:**
- ✅ **Google Colab** (Seamless cloud execution for notebooks)
- ✅ **VS Code** (Primary IDE for development & local execution)
- ✅ **Windows 10 + PowerShell** (Local environment configuration)
- ❌ **R Code** (Omitted entirely to maintain a pure Python focus)

---

## 📚 Chapter Progress

| Chapter | Topic | Status | Primary Notebook |
|:---|:---|:---:|:---|
| **[1](./chapter_01_exploratory_data_analysis/)** | Exploratory Data Analysis | ⬜ Not Started | [`01_eda.ipynb`](./chapter_01_exploratory_data_analysis/01_eda.ipynb) |
| **[2](./chapter_02_data_distribution/)** | Data & Sampling Distributions | ⬜ Not Started | [`02_data_distribution.ipynb`](./chapter_02_data_distribution/02_data_distribution.ipynb) |
| **[3](./chapter_03_statistical_experiments/)**| Statistical Experiments & Significance Testing| ⬜ Not Started | — |
| **[4](./chapter_04_regression_classification/)**| Regression & Prediction | ⬜ Not Started | — |
| **[5](./chapter_05_classification/)** | Classification | ⬜ Not Started | — |
| **[6](./chapter_06_probability/)** | Probability Distributions | ⬜ Not Started | — |
| **[7](./chapter_07_statistical_machine_learning/)**| Statistical Machine Learning | ⬜ Not Started | — |

> **Legend:** ✅ Completed | 🔄 In Progress | ⬜ Not Started

---

## 🚀 Quick Start Guide

### Option 1: Google Colab (Recommended for Zero Setup)
1. Navigate to any `*.ipynb` file in this repository.
2. Click the **"Open in Colab"** badge at the top of the file, or upload it directly to [Colab](https://colab.research.google.com).
3. *(Optional)* Go to `Runtime` → `Change runtime type` → Select `GPU` for machine learning chapters.
4. Run the cells sequentially. 

### Option 2: Local Environment (Windows 10 + PowerShell)

**Prerequisites:** Python 3.12+, VS Code (with Jupyter extension), and Git.

```powershell
# 1. Clone the repository
git clone [https://github.com/beingAnujChaudhary/Practical-Statistics-for-DS-.git](https://github.com/beingAnujChaudhary/Practical-Statistics-for-DS-.git)
cd Practical-Statistics-for-DS-

# 2. Create and activate a virtual environment
python -m venv venv
.\venv\Scripts\Activate.ps1

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch VS Code
code .

```

*(Note: If you prefer Conda, use `conda env create -f environment.yml` followed by `conda activate psds-python`)*

---

## 🧰 Tools & Libraries

| Category | Core Libraries |
| --- | --- |
| **Data Manipulation** | `pandas`, `numpy` |
| **Visualisation** | `matplotlib`, `seaborn`, `plotly` |
| **Statistics** | `scipy`, `statsmodels` |
| **Machine Learning** | `scikit-learn`, `xgboost`, `lightgbm` |
| **Utilities** | `jupyter`, `ipywidgets`, `tqdm`, `joblib` |

---

## 📝 Repository Workflow

To get the most out of this repository, follow this structured approach for each chapter:

1. **Read** the corresponding chapter in the textbook.
2. **Execute** the main notebook (`0X_chapter_name.ipynb`) cell-by-cell to understand the core code.
3. **Practise** by completing the end-of-chapter tasks in `exercises.ipynb`.
4. **Explore** and extend the concepts with your own data in `experiments.ipynb`.
5. **Summarise** the key insights, formulas, and takeaways in `chapter_notes.md`.
6. **Commit** your progress using descriptive Git messages.

**Standard Notebook Template:**

```python
# %% [markdown]
# # Chapter X: [Title]
# **Source**: Practical Statistics for Data Scientists, 3e, pp. XX-XX

# %%
# Import utilities and standardise visualisations
from utils.notebook_setup import *

# %%
# Load processed data for analysis
df = pd.read_csv('../datasets/processed/cleaned_data.csv')

```

---

## 🗂️ Data Management

Strict data management rules are enforced to ensure reproducibility and keep the repository lightweight:

* **`datasets/raw/`**: Original, immutable downloads. Never modify these directly. *(Note: Large files are ignored via `.gitignore`)*.
* **`datasets/processed/`**: Cleaned, analysis-ready datasets. Notebooks should always load data from here.
* **`datasets/external/`**: Third-party supplementary data with proper source attribution.

---

## 📂 Directory Structure

```text
Practical-Statistics-for-DS/
│
├── README.md                 # Project overview
├── requirements.txt          # Python dependencies (pip)
├── environment.yml           # Conda environment definition
├── .gitignore                # Git ignore rules
├── LICENSE                   # MIT License
│
├── assets/                   # Visual assets (covers, diagrams, banners)
├── datasets/                 # Global datasets (raw, processed, external)
├── notes/                    # Global study notes, formulas, and cheatsheets
├── utils/                    # Reusable Python helper scripts (plotting, stats)
│
├── chapter_01_exploratory_data_analysis/
│   ├── 01_eda.ipynb          # Main chapter implementation
│   ├── chapter_notes.md      # Markdown summary of key takeaways
│   ├── exercises.ipynb       # Python solutions to book exercises
│   ├── experiments.ipynb     # Personal extensions and sandbox
│   ├── datasets/             # Chapter-specific datasets
│   └── output/               # Generated graphs and tables
│
├── chapter_02_data_distribution/
│   └── ... (Consistent structure across all chapters)
│
└── output/                   # Global output for final, publication-ready plots

```

---

## 🤝 Contributing & Disclaimer

While this is a personal learning repository, collaboration is welcome! Feel free to fork the project for your own studies, or open an issue if you spot an error in the implementation.

> ⚠️ **Disclaimer**: This repository is strictly for educational purposes. All rights to the original text, conceptual examples, and proprietary datasets belong to the authors and O'Reilly Media. Please support the authors by purchasing *[Practical Statistics for Data Scientists, 3rd Edition](https://www.oreilly.com/library/view/practical-statistics-for/9781492072942/)*.

---

## 👤 Author

**Anuj Chaudhary** 🔗 [GitHub](https://github.com/beingAnujChaudhary) | ✉️ [Email

```

```
