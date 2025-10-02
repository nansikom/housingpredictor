# Chennai Property Sale Price Prediction 🏘️

## Description
This project implements a **Deep Learning Regression Model** using TensorFlow/Keras to accurately predict house sale prices in Chennai, India, based on a dataset containing 22 property and sales attributes. The workflow covers end-to-end data science tasks, from comprehensive data cleaning and exploratory data analysis (EDA) to feature engineering and model training.

---

## Setup
To run this project locally, you need Python and several data science libraries.

### Prerequisites
* Python 3.8+
* Git (for cloning)

### Installation
1.  **Clone the repository:**
    ```bash
    git clone git@github.com:nansikom/housingpredictor.git
    cd housingpredictor
    ```

2.  **Install the necessary libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
    ```

---

## Usage

### 1. Data Preparation
The project assumes the raw data file, `Chennai houseing sale.csv`, is available in the appropriate input path as used in the notebook.

### 2. Training the Model
Run the primary Python script or Jupyter Notebook (which contains the code snippets provided) to execute the full workflow:
* Data cleaning (interpolation, feature renaming).
* Feature engineering (`age`, `month`, `year` creation).
* Data splitting and scaling (`MinMaxScaler`).
* Model training (Neural Network fit for 400 epochs).

### 3. Making Predictions
The final model can be used to predict the sale price for a new, single property, provided its features are scaled using the fitted `MinMaxScaler`.

---

## Key Features

* **Robust Data Cleaning:** Handled over 50 missing values via interpolation and standardized inconsistent categorical labels (e.g., 'Chrompt' to 'Chrompet').
* **Effective Feature Engineering:** Calculated property age and extracted time-series features (`month`, `year`) to improve predictive power.
* **Comprehensive EDA:** Utilized correlation matrices and heatmaps to identify the **Registration Fee (0.88)** and **Indoor Square Footage (0.61)** as the strongest drivers of sale price.
* **Deep Learning Model:** A Sequential Neural Network was trained, achieving an **Explained Variance Score of 0.92**, demonstrating high predictive accuracy on the test set.

---

## Technologies Used

| Category | Tool / Library | Purpose |
| :--- | :--- | :--- |
| **Data Processing** | Python, Pandas, NumPy | Data loading, manipulation, and numerical operations. |
| **Visualization** | Matplotlib, Seaborn | Exploratory data analysis, plotting distributions, and correlations. |
| **Machine Learning** | Scikit-learn | Data splitting (`train_test_split`), feature scaling (`MinMaxScaler`), and model evaluation. |
| **Deep Learning** | TensorFlow / Keras | Defining, compiling, and training the Neural Network regression model. |

---

**Project Adopted from: Chennai Property sale price Prediction**
