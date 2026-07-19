# Introduction to Machine Learning for Social Scientists

**Southampton Statistics Summer School** | 30 July 2026  
**Instructor:** Brody Hannan, University of Southampton

A 2-hour workshop introducing machine learning to PhD-level social scientists with a background in traditional statistics. No prior ML or Python experience required.

---

## Workshop Structure

| Part | Duration | Format |
|---|---|---|
| Theory lecture | 45 min | Beamer slides (PDF) |
| Hands-on practical | 75 min | Google Colab notebook |

---

## Repository Contents

```
introduction-to-machine-learning/
├── slides/
│   ├── intro_ml_ssss.tex     # LaTeX source (Beamer/Metropolis)
│   └── intro_ml_ssss.pdf     # Compiled PDF (see Releases)
├── notebook/
│   └── ml_workshop.ipynb     # Google Colab notebook (Python)
├── data/
│   └── (data loads automatically in the notebook)
└── README.md
```

---

## The Dataset

**1994 US Census Income** (UCI Adult dataset)

- 48,842 adult respondents
- Task: predict whether income exceeds $50K/year
- Features: age, education, occupation, marital status, sex, race, hours worked per week, country of origin
- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/2/adult) via `scikit-learn`

The dataset is loaded automatically in the notebook. No manual download required.

This dataset appears in [awesomedata/awesome-public-datasets](https://github.com/awesomedata/awesome-public-datasets) under Social Sciences.

---

## What the Practical Covers

1. **Data loading and exploration** -- descriptive statistics, class distributions, missing values
2. **Preprocessing** -- encoding categorical variables, train/test split
3. **Decision tree** -- build, visualise, evaluate
4. **Random forest** -- build, evaluate, interpret variable importance
5. **Gradient boosting** -- build, compare against previous models
6. **Extension: K-means clustering** -- discover sociodemographic groups in the census data

---

## How to Use the Notebook

### Option 1: Google Colab (recommended)

Click the badge below or open the link:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/BHannan01/introduction-to-machine-learning/blob/main/notebook/ml_workshop.ipynb)

No installation needed. Requires a Google account.

### Option 2: Run locally

```bash
git clone https://github.com/BHannan01/introduction-to-machine-learning.git
cd introduction-to-machine-learning
pip install -r requirements.txt
jupyter notebook notebook/ml_workshop.ipynb
```

Required packages: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

---

## Compiling the Slides

The slides use the [Metropolis Beamer theme](https://github.com/matze/mtheme). Requires a recent TeX Live or MikTeX installation.

```bash
cd slides
pdflatex intro_ml_ssss.tex
pdflatex intro_ml_ssss.tex  # run twice for cross-references
```

Or use Overleaf: upload `intro_ml_ssss.tex` and compile with pdfLaTeX.

---

## Prerequisites for Participants

- A Google account (for Colab)
- Basic familiarity with statistical concepts (regression, hypothesis testing)
- No Python or ML experience required

---

## License

Materials are shared for educational use. The dataset is publicly available from the UCI ML Repository (Dua, D. and Graff, C., 2019).
