
# Lab 01 — Environment Setup: Report

**Student:** Alisha Izhar
**Repository:** https://github.com/alishaizhar/ai-lab-portfolio

## 1. Installation Evidence

- Anaconda version: conda 25.1
- Python (base): 3.13.5
- `ai-lab` environment created with Python 3.11.16
- Git version: 2.55.0.windows.5
- pandas version: 3.0.5

## 2. Dataset Inspection (Titanic dataset)

**Shape:** 891 rows x 15 columns

**Missing values:**

deck 688 (77.2%)
age 177 (19.9%)
embarked 2 (0.2%)
embark_town 2 (0.2%)


**Coefficient of variation (std/mean), largest first:**

parch 2.112
sibsp 2.108
fare 1.543
survived 1.268
age 0.489
pclass 0.362


**Answer:** `parch` has the largest coefficient of variation, meaning its values are the most spread out relative to their own average. Without scaling, models based on distance or magnitude (like KNN or linear regression) might wrongly treat `parch` as more important, simply because its scale is more spread out — not because it is actually the most predictive.

## 3. Git Graph
42368a7 (HEAD -> main, origin/main, origin/HEAD) Merge pull request #1 from alishaizhar/lab01/homework
|
| * fb8a41b (origin/lab01/homework, lab01/homework) Add inspect.py with fixed path_or_url bug and tested on two datasets
|/
9970221 Lab 01: environment setup and first notebook

## 4. Home Assignment

`lab01/inspect.py` contains a generic `inspect(path_or_url)` function, fixed to accept any CSV path/URL (previously hardcoded to Titanic). Tested successfully on two datasets:
1. Titanic dataset (891 rows, 15 columns)
2. Tips dataset (244 rows, 7 columns)

Merged via Pull Request #1: https://github.com/alishaizhar/ai-lab-portfolio/pull/1