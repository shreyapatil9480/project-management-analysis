# Project Management Analysis

This repository contains a **synthetic dataset** and a comprehensive analysis notebook designed for practicing the skills of a **business analyst**, **program manager**, or **data analyst**.  The project demonstrates how to perform exploratory data analysis (EDA), data visualization and build a predictive model using Python.  It is designed to be ready‑to‑use out of the box with no external dependencies beyond the libraries listed in `requirements.txt`.

## Contents

- `synthetic_project_data.csv` – A synthetic dataset of 500 projects with fields such as start/end dates, budget, team size, complexity level, manager experience, client satisfaction, quality score, whether the project was delayed, and whether it was ultimately successful.
- `analysis.ipynb` – A Jupyter notebook that performs exploratory data analysis, creates visualizations and builds a predictive model for project success.
- `requirements.txt` – A list of Python packages needed to run the notebook.

## Dataset Description

The dataset is entirely synthetic and was generated to mimic typical project management scenarios.  Each row represents a project.  Below is a description of the columns:

| Column | Description |
|---|---|
| `ProjectID` | Unique identifier for each project. |
| `StartDate` | Project start date (YYYY‑MM‑DD). |
| `EndDate` | Project end date (YYYY‑MM‑DD). |
| `DurationDays` | Number of days between start and end. |
| `Budget` | Project budget in USD. |
| `TeamSize` | Number of people involved in the project. |
| `ComplexityLevel` | Ordinal measure of project complexity (1–5). |
| `ManagerExperienceYears` | Years of experience of the project manager. |
| `ClientSatisfaction` | Client satisfaction score (1–10). |
| `QualityScore` | Quality score of delivered product (0.0–1.0). |
| `Delayed` | Whether the project ran longer than 180 days (1 = Yes, 0 = No). |
| `Success` | Binary flag indicating if the project was considered successful (1 = Yes, 0 = No). |

Because the dataset is synthetic, there is no private or proprietary information contained in it.

## Running the Analysis

To explore the data and reproduce the analysis:

1. **Clone the repository** (or download it) to your local machine.
2. Install the required packages (preferably in a virtual environment):
   ```bash
   pip install -r requirements.txt
   ```
3. Start Jupyter Notebook and open `analysis.ipynb`:
   ```bash
   jupyter notebook
   ```
4. Run the notebook cells in order.  The notebook will:
   - Load and display the first few rows of the dataset.
   - Provide summary statistics.
   - Visualize distributions (e.g. budgets, success rates, quality scores).
   - Compute and display a correlation heatmap.
   - Build and evaluate a logistic regression model to predict project success.

The notebook uses a train/test split and reports accuracy, a classification report and a confusion matrix.  Feel free to experiment with other models (e.g. decision trees, random forests) to improve performance.

## Getting Started Without Jupyter

If you prefer to run the analysis from a script instead of a notebook, you can adapt the code from `analysis.ipynb` into a Python script.  The dataset is in CSV format and can be loaded using `pandas`.

## Contributing

This project is intended as a learning resource.  If you would like to expand on the dataset, add more visualizations or experiment with additional models, feel free to fork the repository or open a pull request.

## License

The contents of this repository are provided for educational purposes.  You are free to use and modify this project for your own learning or portfolio.
