# Video Game Sales Prediction Using Machine Learning

## Project Overview

This project analyzes historical video game sales data and predicts global sales using machine learning regression models. It also explores sales trends across genres, platforms, and release years.

## Machine Learning Algorithms

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

## Project Workflow

1. Import Python libraries.
2. Upload and load the video game sales dataset.
3. Inspect the first and last records, dataset dimensions, columns, data types, and statistical summaries.
4. Check missing values, duplicate records, and missing-value percentages.
5. Clean the dataset and save the cleaned data.
6. Perform exploratory data analysis:
   - Global sales distribution
   - Genre-wise sales
   - Year-wise sales
   - Platform-wise sales
7. Select input features and the target variable.
8. Preprocess numerical and categorical columns using imputation and one-hot encoding.
9. Split the data into training and testing sets.
10. Train and evaluate Linear Regression, Decision Tree, and Random Forest models.
11. Compare model metrics.
12. Perform 5-fold cross-validation.
13. Tune Decision Tree and Random Forest hyperparameters using GridSearchCV.
14. Generate sales predictions and convert them into Low Sales / High Sales categories for confusion-matrix analysis.
15. Evaluate final models, select the best model, and save the model and result files.

## Dataset

The notebook expects a file named:

`vgsales.csv`

The CSV is not included in this repository package. When running in Google Colab, the notebook will prompt you to upload `vgsales.csv`. Use a dataset copy that you are permitted to use and redistribute. If you publish the dataset separately, include its original source and license information here.

The notebook expects these columns from the dataset:

- `Rank`
- `Name`
- `Platform`
- `Year`
- `Genre`
- `Publisher`
- `NA_Sales`
- `EU_Sales`
- `JP_Sales`
- `Other_Sales`
- `Global_Sales`

## Requirements

- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib
- Jupyter Notebook (optional if using Google Colab)

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Select **File → Upload notebook**.
3. Upload `Video_Game_Sales_Prediction.ipynb`.
4. Run the notebook from top to bottom.
5. When the dataset upload cell appears, select `vgsales.csv`.
6. Continue running the remaining cells.

## Run Locally

1. Clone or download this repository.
2. Place `vgsales.csv` in the working directory.
3. Install dependencies with `pip install -r requirements.txt`.
4. Start Jupyter with `jupyter notebook`.
5. Open `Video_Game_Sales_Prediction.ipynb` and run all cells in order.

## Generated Outputs

The notebook creates cleaned data and model-evaluation artifacts during execution, including:

- `vgsales_cleaned.csv`
- Cross-validation and model-comparison CSV files
- Confusion-matrix CSV files
- A saved best-model file under `project_results/`
- `Video_Game_Sales_Prediction_Results.zip`

These are generated when the notebook is run; they are not precomputed in this repository.

## Repository Structure

```text
Video-Game-Sales-Prediction/
├── Video_Game_Sales_Prediction.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Author

**Name:** Add your name  
**Course / Semester:** Add your course and semester  
**College:** Add your college name

## Disclaimer

This is an academic machine learning project. Model performance depends on the dataset, data quality, feature selection, and train/test split. Actual evaluation results are produced by running the notebook.
