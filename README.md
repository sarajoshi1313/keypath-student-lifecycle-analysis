# Keypath Student Lifecycle Analysis

This repository contains two public datasets and a Jupyter notebook analysing student dropout risk and post-graduation career success. It applies and compares two machine learning models — Random Forest and kNN, to explore predictive patterns across the student lifecycle, as part of a data science career task for a Data Scientist role at Keypath Education.

- **Section 1 — Dropout risk:** Random Forest classifier, with a tuned decision threshold (0.4) chosen to prioritise recall.
- **Section 2 — Career success:** kNN classifier (k=5) with scaled features.
- Both models are evaluated using precision, recall, F1-score, and ROC-AUC rather than plain accuracy, due to class imbalance in section 1 and to allow direct comparison.

## Data

### Dataset 1: Students' Dropout and Academic Success Dataset

| | |
|---|---|
| **Size** | 4,424 records |
| **Columns** | 37 |
| **URL** | [Students' Dropout and Academic Success Dataset](https://www.kaggle.com/datasets/mahwiz/students-dropout-and-academic-success-dataset?resource=download) |

**Description:** This dataset includes information on students' academic paths, demographics, and socio-economic factors at the time of enrolment, as well as students' academic performance at the end of the first and second semesters.

### Dataset 2: Education and Career Success

| | |
|---|---|
| **Size** | 400 records |
| **Columns** | 19 |
| **URL** | [Education and Career Success](https://www.kaggle.com/datasets/adilshamim8/education-and-career-success/data) |

**Description:** This dataset explores how students' academic achievements, skills, and extracurricular activities translate into real-world career outcomes by combining educational metrics with practical experience.

## Getting Started

1. **Download this repository**

  Simply download the `.ipynb` file and both dataset CSVs directly from this repo.

2. **Install the required packages**
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

3. **Open the notebook**
   Launch Jupyter Notebook or JupyterLab, then open `keypath_student_lifecycle_analysis.ipynb`. Alternatively, upload the notebook and datasets to [Google Colab](https://colab.research.google.com/) to run it in the browser with no local setup.

4. **Run the cells**
   Make sure both dataset CSVs are in the same folder as the notebook, then run all cells in order (`Kernel > Restart & Run All`) to reproduce the cleaning, exploration, modelling, and evaluation steps.
