# Product Category Prediction

This project aims to predict product categories using a dataset from Kaggle. The dataset includes various features like 'Original Price', 'Offer Price', 'Discount', 'Reviews', and 'Product Name'.

## Dataset Information

The dataset is sourced from Kaggle and includes detailed product information:
- `Original Price`
- `Offer Price`
- `Discount`
- `Reviews`
- `Product Name`
- `Category`

[Link to Dataset](https://www.kaggle.com/datasets/pankajsharma127/nykaa-products-2023)

## Project Steps

### 1. Data Collection and Preprocessing
- Collect the dataset containing product information, including features like 'Original Price', 'Offer Price', 'Discount', 'Reviews', and 'Product Name'.
- Preprocess the dataset by handling missing values, extracting numeric values from text columns, and encoding categorical variables.

### 2. Exploratory Data Analysis (EDA)
- Explore the distribution of numerical features (e.g., 'Original Price', 'Offer Price', 'Reviews') using histograms and box plots.
- Investigate relationships between features using scatter plots and correlation matrices.
- Analyze the distribution of product categories to identify any class imbalances.

### 3. Feature Engineering
- Select relevant features for prediction, including numerical features related to pricing and reviews, and the textual feature 'Product Name'.
- Generate polynomial features of degree 2 to capture potential nonlinear relationships.

### 4. Data Splitting
- Split the dataset into training and testing sets using the `train_test_split` function, allocating around 80% of the data for training and 20% for testing.

### 5. Feature Scaling
- Standardize the polynomial features using `StandardScaler` to ensure all features have a mean of 0 and a standard deviation of 1.

### 6. Model Training
- Train a machine learning model, such as Logistic Regression, using the scaled polynomial features and the target variable ('Category').
- Fit the model to the training data to learn the underlying patterns between the features and the target variable.

### 7. Model Evaluation
- Evaluate the trained model's performance using classification metrics like precision, recall, and F1-score.
- Analyze the classification report to understand the model's predictive performance for each product category.

## How to Run

1. **Setup**:
   - Ensure you have Python installed on your system.
   - Clone the repository and navigate to the project directory.

2. **Dependencies**:
   - Install necessary dependencies. You might use `pip` to install required packages:
     ```sh
     pip install -r requirements.txt
     ```

3. **Running the Scripts**:
   - Execute the data processing and model training script:
     ```sh
     python main.ipynb
     ```

4. **Prediction**:
   - Follow the instructions in the script to input product details and make predictions.


