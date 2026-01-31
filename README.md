# red-wine-supernova
Overview:
    This project explores the chemical profiles of red and white wines to determine which factors most significantly influence quality ratings. By leveraging various predictive models, the analysis aims to identify whether we can accurately forecast a wine's "quality score" based solely on objective laboratory measurements.

Data:
    The project utilizes the Wine Quality Dataset (available via the UCI Machine Learning Repository).
    Source Files: winequality-red.csv and winequality-white.csv are stored in the data_raw/ directory to ensure data integrity and provenance.
    Processing: All data cleaning, feature engineering (e.g., creating a "color" dummy variable), and exploratory data analysis (EDA) are performed within the main Jupyter Notebook (.ipynb).
    Both the winequality files (red and white) are in a data_raw file, since both of them are untouched. They are modified and expanded upon in the ipynb document.

Environment Setup:
    To run this analysis, you will need Python 3.x and the following libraries:
    Data Manipulation: pandas, numpy
    Visualization: matplotlib, seaborn
    Machine Learning: scikit-learn
    Type pip install pandas numpy matplotlib seaborn scikit-learn for a quick run

How to reproduce a result:
    git clone https://github.com/your-username/red-wine-supernova.git
    Ensure the data_raw/ folder contains the original CSV files.
    Open the .ipynb file in Jupyter Lab or VS Code and select "Run All."

Troubleshooting/known issues:
    Imbalanced Classes: The dataset contains significantly more "average" quality wines (scores 5-6) than exceptional or poor ones, which may bias the predictors.
    Correlated Features: High correlation between density and alcohol or fixed acidity and pH can cause multicollinearity issues in simple linear models.
    Missing Files: If you receive a FileNotFoundError, ensure your working directory is set to the project root so the script can see the data_raw/ folder.
