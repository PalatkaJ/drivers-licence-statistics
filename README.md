# Driver's License Test Statistics

This repository contains a statistical analysis of driver license test outcomes based on a dataset of applicants and their practical/theoretical test scores. The project investigates whether demographic factors such as age, gender, race, and training influence the final result of the driving exam.

The analysis is implemented in a Jupyter notebook and uses Python libraries for data processing, hypothesis testing, visualization, and statistical inference.

## Project goal

The main questions explored in this project are:

- Does gender affect the probability of passing the driving test?
- Does age group influence test performance?
- Is there a relationship between race and exam outcome?
- Does prior training improve the likelihood of passing?
- Which aspects of the driving test are most affected by age and preparation?

## Dataset

The project uses the dataset:

- `data/drivers_licence_data.csv`

The dataset includes applicant information and performance metrics such as:

- Applicant ID
- Gender
- Age Group
- Race
- Training level
- Practical driving skills scores (signals, yield, speed control, night drive, road signs, steering, mirror usage, parking, etc.)
- Theory test score
- Final qualification status (`Yes` / `No`)

## Repository structure

```text
.
├── data/
│   └── drivers_licence_data.csv
├── statistics_project.ipynb
├── README.md
├── .gitignore
└── .DS_Store
```

## What is analyzed in the notebook?

The notebook includes:

- Data loading and exploratory analysis
- Summary statistics and data inspection
- Contingency tables for categorical variables
- Chi-square tests for independence
- ANOVA tests for comparing score distributions by age group
- Visualizations of score differences across age groups
- Confidence interval estimation for mean parking performance
- Interpretation of the statistical results

## Statistical methods used

The project applies common inferential statistics such as:

- Chi-square test of independence
- One-way ANOVA
- Confidence intervals for a population mean
- Descriptive statistical summaries and plots

## Requirements

To run the notebook, install the following dependencies:

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

## Run locally

Clone the repository and start Jupyter:

```bash
git clone https://github.com/PalatkaJ/drivers_licence_statistics.git
cd drivers_licence_statistics
jupyter notebook
```

Then open `statistics_project.ipynb`.

## Key findings

The analysis suggests that:

- Gender does not have a statistically significant effect on the final test result.
- Race also does not show a significant effect on passing status.
- Age group is associated with different outcomes, especially in practical driving tasks.
- Training has a strong and statistically significant effect on passing probability.
- Younger applicants (especially teenagers) tend to perform worse in practical tasks, while theory test performance remains relatively similar across age groups.

## Data source

This project is based on a publicly available dataset from Kaggle related to driver license test scores.

## Author

- Jan Palatka

## Course

- Probability and Statistics 1

## License

This project is intended for educational and research purposes.
