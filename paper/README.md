# MATH261A-project

Author: Yena Jeon

First-version submission date: September 25, 2026

This project asks how well first-half time predicts second-half time and whether runners maintained the same average pace across the two halves of the 2023 Boston Marathon. Simple linear regression is the main analysis, with a paired t-test of the mean second-half minus first-half difference as a supplementary analysis.


## Data

Data used in this project were obtained from the SCORE Sports Data Repository, which lists the Boston Athletic Association as the original source.
No specific license for this dataset is stated on the SCORE Sports Data Repository page.
[SCORE: 2023 Boston Marathon runners](https://data.scorenetwork.org/running/boston_marathon_2023.html)

## Files and reproduction

- `paper/paper-v1.qmd`: report text and analysis code.
- `paper/paper-v1.pdf`: rendered report.
- `paper/references.bib`: data and software references.
- `data/`: external CSV, excluded from Git. The QMD downloads it if absent.

Open `MATH261A-project.Rproj` in RStudio, open the QMD, and run its chunks from top to bottom or click Render. `_quarto.yml` sets the working directory to the project root. The code uses tidyverse, ggpubr, sandwich, and knitr. Quarto and a LaTeX installation are required for the PDF.

`boston-lm` fits the regression, `tbl-predictions` calculates example predictions, `prediction-check` evaluates an 80/20 split with seed 261, and `paired-pace-test` compares the two times from each runner. `summary(lm_fit)` tests a zero regression slope; `pace_test` tests a zero average within-runner time difference. They answer different questions. The current report does not test a slope of one.

## External resources

ChatGPT was used for preliminary research and troubleshooting R/Quarto code. OpenAI Codex also assisted with the analysis code and report drafting, including the revised prediction question, paired t-test, and PDF rendering. This is an assisted draft for the author to review and rewrite in accordance with the assignment's student-authorship requirement.
The R/Quarto code referred to the provided template code and course materials.
Information about the dataset was obtained from the SCORE Sports Data Repository.
