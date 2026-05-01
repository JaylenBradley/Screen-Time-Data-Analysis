# Screen Time and Mental Wellness Analysis

## Project Description

This project investigates the relationship between daily screen usage and various measures of mental and physical well-being. Using data from a survey of 400 participants, the analysis explores how different types of screen time (work vs. leisure) correlate with stress levels, sleep quality, productivity, and overall mental wellness.

The repository includes the full data cleaning process, exploratory data analysis (EDA), and preliminary visualizations to establish a baseline for understanding how digital habits impact modern life.

## Data Source

The dataset was collected via a survey of 400 participants conducted by **Adharshini Kumaresan** (approximately late 2024/early 2025). \* **Dataset Link:** [Kaggle: Screen Time vs Mental Wellness Survey 2025](https://www.kaggle.com/datasets/adharshinikumar/screentime-vs-mentalwellness-survey-2025)

## Data Dictionary / Codebook

| Variable | Type | Description |
|:-----------------------|:-----------------------|:-----------------------|
| `user_id` | String | Unique identifier for each survey participant. |
| `age` | Numeric | Age of the participant (Range: 16–60 years). |
| `gender` | Factor | Gender identity (Female, Male, Non-binary/Other). |
| `occupation` | Factor | Employment status (Unemployed, Student, Self-employed, Employed, Retired). |
| `work_mode` | Factor | Work environment (Remote, Hybrid, In-person). |
| `screen_time_hours` | Numeric | Total daily screen time across all devices (Mobile, Laptop, TV). |
| `work_screen_hours` | Numeric | Daily screen time spent specifically on work or study tasks. |
| `leisure_screen_hours` | Numeric | Daily screen time spent on social media, streaming, gaming, etc. |
| `sleep_hours` | Numeric | Average duration of sleep per night in hours. |
| `sleep_quality_1_5` | Integer | Self-reported sleep quality on a scale of 1 (Poor) to 5 (Excellent). |
| `stress_level_0_10` | Numeric | Self-reported stress level on a scale of 0 to 10. |
| `productivity_0_100` | Numeric | Self-reported productivity score on a scale of 0 to 100. |
| `exercise_min_per_week` | Numeric | Total minutes of physical exercise per week. |
| `social_hours_per_week` | Numeric | Hours spent socializing offline per week. |
| `wellness_index_0_100` | Numeric | Calculated mental wellness index on a scale of 0 to 100. |

## Key Findings from EDA

-   **Age Range:** Most participants are in their 20s to late 30s.
-   **Screen Habits:** The average daily screen time is approximately 8–10 hours, with a significant portion (avg \~7 hours) dedicated to leisure.
-   **Work vs. Leisure:** Work-related screen time is skewed right, with most participants spending only 0–2 hours on work-specific screen tasks.
-   **Social Trends:** A concerning number of participants reported 0 hours of offline social interaction per week.

## Repository Structure

-   `data/`: Contains the raw `.csv` and cleaned `.rds` data files.
-   `cleaning-eda.qmd`: The Quarto document containing the R code for data processing and visualization.
-   `written-report.qmd`: Final analysis and interpretations.
-   `presentation.pdf`: Summary of findings for stakeholders.

## How to Run

1.  Ensure you have [Quarto](https://quarto.org/) and R installed.
2.  Install required R packages: `tidyverse`, `ggplot2`.
3.  Run `quarto preview cleaning-eda.qmd` to view the analysis.
