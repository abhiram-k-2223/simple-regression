# Parkinson's Disease Progression Prediction

This project aims to predict the progression of Parkinson's disease using a linear regression model. The dataset used is a Parkinson's disease dataset, and the target variable is 'PPE' (a biomedical voice measurement). The workflow includes data loading, preprocessing with scaling, and model training and evaluation.

## Project Description

### Data Loading

The dataset is loaded using pandas, providing an initial look at the data to understand its structure and content. The target variable 'PPE' is identified for prediction.

### Data Splitting

The dataset is split into training and testing sets using an 80-20 split. This helps in evaluating the model's performance on unseen data. The target variable 'PPE' is separated from the feature set.

### Data Preprocessing

#### Scaling with StandardScaler

Numerical features are scaled using StandardScaler to ensure they have zero mean and unit variance. This step is crucial for linear regression models to ensure that the features contribute equally to the result and improve the model's convergence during training.

### Model Training

A linear regression model is trained on the scaled training data. Linear regression is a simple yet powerful model for predicting continuous outcomes, making it suitable for predicting the 'PPE' values in this dataset.

### Prediction

The trained model is used to predict 'PPE' values on the test data. The predicted values are then compared to the actual values to assess the model's performance.

### Evaluation

The model's performance is evaluated using the R² score, which indicates the proportion of variance in the dependent variable that is predictable from the independent variables. A higher R² score signifies a better fit of the model to the data.

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/abhiram-k-2223/simple-regression.git
    cd simple-regression
    ```

2. **Install dependencies**:
    ```bash
    pip install pandas scikit-learn
    ```

3. **Run the Jupyter notebook or script**:
    - If using a Jupyter notebook, open `simple_regression.ipynb` and run the cells sequentially.

4. **Output**:
    - The R² score indicating the model's performance on the test set.

This project demonstrates how to preprocess data, scale features, and train a linear regression model to predict the progression of Parkinson's disease effectively.
