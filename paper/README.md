# MATH261A-project

Author: Yena Jeon

First-version submission date: September 25, 2026

Final-version submission date: October 30, 2026

This project asks how well first-half time predicts second-half time and whether runners maintained the same average pace across the two halves of the 2023 Boston Marathon. Simple linear regression is the main analysis, with a paired t-test of the mean second-half minus first-half difference as a supplementary analysis.

## Project structure

- `paper/paper-final_yena_jeon.qmd`: final Quarto report source, including the R analysis code.
- `paper/paper-final_yena_jeon.pdf`: rendered final report.
- `paper/references.bib`: BibTeX references used in the report.
- `paper/ieee.csl`: IEEE numeric citation style used for citations and the reference list.
- `data/`: local data directory used during rendering; the report source downloads the dataset if it is missing.
- `_quarto.yml`: project-level rendering and citation settings.

## Data

Data used in this project were obtained from the SCORE Sports Data Repository, which lists the Boston Athletic Association as the original source. No specific license for this dataset is stated on the SCORE Sports Data Repository page.

[SCORE: 2023 Boston Marathon runners](https://data.scorenetwork.org/running/boston_marathon_2023.html)

## External resources

I wrote all R analysis code and developed the statistical analysis. ChatGPT was used to refine English wording and improve clarity and to assist with Quarto formatting and PDF rendering. I reviewed and wrote the final text and code.

The Quarto document was based on the provided course template and course materials. Information about the dataset was obtained from the SCORE Sports Data Repository.
