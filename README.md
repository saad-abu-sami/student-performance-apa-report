# Student Performance: APA-style Statistical Report

Five analyses in R on the UCI Student Performance data (395 maths students):
Welch t-test, one-way ANOVA with Tukey, Pearson correlation,
multiple regression, and chi-square.

## Key results
- Internet vs no internet, final grade: t(94.22) = -1.99, p = .050, d = 0.26 (borderline)
- Study time and final grade: F(3, 391) = 1.73, p = .161
- First and final grade: r(393) = .80
- Regression (study time, absences, failures): R² = .135; failures is the main predictor
- School and internet access: χ²(1) = 7.05, p = .008, V = .13

## Files
- `02_student_report.Rmd`: the report source
- `Student_Performance_Statistical_Analysis_Report.pdf`: the rendered report
- `student.csv`: cleaned data
- `r-ground-truth.json`: R results used to check the report

## Render
1. Install R 4.6 and RStudio.
2. Run `install.packages(c("rmarkdown", "knitr", "ggplot2", "jsonlite"))`.
3. Put the data in the same folder and run `rmarkdown::render("02_student_report.Rmd")`.

## Data credit
UCI Student Performance (Cortez, 2008), CC BY 4.0. https://doi.org/10.24432/C5TG7T
