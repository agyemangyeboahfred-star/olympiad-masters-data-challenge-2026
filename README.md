# Milan Cortina 2026 Olympiad: Athlete Performance Analysis

This project focuses on analyzing athlete data for the Milan Cortina 2026 Winter Olympics. It involves exploratory data analysis (EDA) to understand athlete characteristics, country-specific performance, and the development of a predictive model to forecast medal outcomes.

## Project Structure

The notebook is structured into several key sections:

1.  **Data Loading and Cleaning**: Initial setup, loading of raw athlete data, and cleaning steps to prepare the dataset for analysis.
2.  **Exploratory Data Analysis (EDA) & Storytelling**: Deep dive into the data through various visualizations and statistical summaries. This includes:
    *   USA vs. Canada medal distribution.
    *   Medal conversion rates between the two countries.
    *   Comparison of athlete quality metrics (e.g., training hours, VO2max).
    *   Sport portfolio analysis, identifying key sports for each country.
    *   Champion profiling to understand attributes of medal winners.
    *   Efficiency analysis: Investment (athletes) vs. Performance (medal rate) by sport.
    *   GDP vs. Medal Performance at a country level.
3.  **Predictive Modeling - Medal vs. No Medal**: Development of a binary classification model to predict whether an athlete will win a medal.
    *   **Preprocessing**: Handling categorical features with OneHotEncoding and numerical features with StandardScaler.
    *   **Train-Test Split**: Dividing the data for model training and evaluation.
    *   **Class Imbalance Handling**: Utilizing SMOTE (Synthetic Minority Over-sampling Technique) to address the imbalance between medal-winning and non-medal-winning athletes.
    *   **Model Training & Evaluation**: Training a Logistic Regression model and assessing its performance using metrics like Accuracy, Precision, Recall, F1-score, and AUC-ROC.
    *   **Confusion Matrix**: Visualizing model performance.
    *   **Precision-Recall Curve**: Evaluating the trade-off between precision and recall.
    *   **Application to Specific Athletes**: Using the trained model to predict medal chances for a selection of notable athletes.

## Data

The project uses the `milan_cortina_2026_athletes.csv` dataset, which contains various attributes of Olympic athletes including their country, sport, physical metrics, training data, and medal outcomes.

## Dependencies

To run this notebook, you will need the following Python libraries:

*   `pandas`
*   `numpy`
*   `matplotlib`
*   `seaborn`
*   `scikit-learn` (sklearn)
*   `imblearn` (imbalanced-learn)

You can install these using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imblearn
```

## How to Run

1.  **Clone the repository** (if applicable) or download the notebook (`.ipynb`) and the `milan_cortina_2026_athletes.csv` file.
2.  **Ensure all dependencies are installed**.
3.  **Place the `milan_cortina_2026_athletes.csv` file** in the same directory as the notebook, or update the `RAW_FILE` path in the notebook.
4.  **Open the notebook** in a Jupyter environment (e.g., Jupyter Lab, VS Code with Python extension, Google Colab).
5.  **Run all cells** sequentially.

## Outputs

The EDA section generates several plots and saves them to the `OUTPUTS/EDA_CHARTS` directory. The cleaned dataset is saved as `cleaned_athletes_dataset.csv` in the `OUTPUTS` directory. The model predictions and evaluation metrics are displayed within the notebook output.
