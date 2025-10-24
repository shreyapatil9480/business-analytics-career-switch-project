# Business Analytics Career Switch Project

This repository contains a **job‑ready analytics project** designed to showcase the skills of a business analyst, program manager or data analyst.  It is suitable for your portfolio and can be used straight out of the box.

## Project Overview

1. **Synthetic Dataset** – A CSV file (`synthetic_project_data.csv`) with 200 simulated projects.  Each row represents a project with realistic features: complexity (1–10), team size, budget (k$), duration (weeks), number of stakeholders, risk score, a binary success indicator and a continuous return‑on‑investment (ROI) percentage.  The data is synthetically generated to mimic typical project management scenarios without exposing any sensitive real‑world information.

2. **Exploratory Data Analysis (EDA)** – The Jupyter Notebook (`analysis.ipynb`) begins with data loading and summary statistics.  It includes histograms for each feature and a correlation heatmap, allowing you to quickly identify relationships between variables.

3. **Predictive Models** – The notebook then tackles two predictive tasks of increasing complexity:
   - **Classification**: A logistic regression model predicts whether a project succeeds based on its attributes.  Accuracy and a confusion matrix are reported.
   - **Regression**: A random forest regressor estimates ROI.  Mean squared error and the R² score assess performance.

4. **Documentation** – The notebook concludes with suggestions for future improvements, such as feature engineering, testing different algorithms, and hyperparameter tuning.

## Repository Structure

```text
business-analytics-career-switch-project/
├── README.md                # You are here
├── requirements.txt         # Python dependencies
├── synthetic_project_data.csv  # Synthetic dataset used in this project
└── analysis.ipynb           # Executable Jupyter Notebook with EDA and models
```

## Getting Started

1. **Clone the repository** (or fork it) to your local machine:

```bash
git clone https://github.com/`<your-username>`/business-analytics-career-switch-project.git
cd business-analytics-career-switch-project
```

2. **Create and activate a virtual environment** (optional but recommended):

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install the required packages**:

```bash
pip install -r requirements.txt
```

4. **Launch the notebook**:

```bash
jupyter notebook analysis.ipynb
```

or use JupyterLab:

```bash
jupyter lab analysis.ipynb
```

The notebook will open in your browser.  Run the cells sequentially to reproduce the analysis, visualizations and predictive models.

## Extending the Project

This repository is intentionally designed to be extensible.  Here are some ideas to take it further:

- **Feature engineering** – Create new variables (e.g., budget per team member, duration per stakeholder) to see if they improve model performance.
- **Algorithm comparison** – Try decision trees, k‑nearest neighbours, support vector machines or gradient boosting for both classification and regression tasks.
- **Cross‑validation & hyperparameter tuning** – Use scikit‑learn’s `GridSearchCV` or `RandomizedSearchCV` to find optimal model settings.
- **Model interpretation** – Explore feature importance in the random forest model or use SHAP values to explain individual predictions.
- **Dashboards** – Build a simple dashboard (e.g., using Plotly Dash or Streamlit) to interactively explore the dataset and models.

## License

This project is released under the MIT License.  Feel free to reuse the code and dataset for educational or portfolio purposes.

## Usage

After launching the notebook, run the cells in sequence to explore the dataset and run the predictive models. The notebook will:

- Display descriptive statistics and histograms for each feature.
- Produce a correlation heatmap to visualize relationships between variables.
- Fit a logistic regression classifier to predict project success and show accuracy and a confusion matrix.
- Fit a random forest regressor to estimate ROI and report the mean squared error (MSE) and the R^2 score.

Feel free to experiment by tuning the models or replacing `synthetic_project_data.csv` with your own data (ensure the column names match or adapt the code accordingly). The analysis notebook is a starting point—you can add new models, features or visualizations as part of your portfolio.
