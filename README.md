# NVIDIA_Hackathon_2024

Welcome to our project for the NVIDIA ODSC Manor Halloween competition! This project focuses on predicting the "scariest monster" based on a global terror poll, where each monster’s scariness is represented by a target variable `y`, which reflects the number of votes each monster received. We utilized advanced data processing, feature engineering, and machine learning techniques to tackle this frightful challenge.

## Competition Overview 🎃

**Challenge:** Predict the target variable `y`—the number of votes each monster received in a global terror poll. We aim to identify the "Scariest Monster of them all" through a regression model with the lowest Root Mean Squared Error (RMSE).

**Dataset:** The dataset includes:
- **11 million monsters**, each with **106 anonymous features** (numerical and categorical).
- Training data (`train.csv`) with labeled examples and target values.

## Solution Approach 🧪

Our approach combines multiple advanced machine learning techniques, including:
1. **Exploratory Data Analysis (EDA):** We examined the data for insights into feature distributions, relationships, and missing values.
2. **Feature Engineering:** We performed feature Selection using XGBoost
3. **Modeling:** We began with linear regression as a baseline, then progressively experimented with tree-based models. XGBoost emerged as the best-performing model, offering a strong balance of accuracy and interpretability for this dataset.
4. **GPU-Acceleration with RAPIDS:** We leveraged GPU-accelerated libraries (`cudf and cuML) for faster data processing, enabling us to handle the dataset size efficiently.

## Model Evaluation and Results 🏆

- **Root Mean Squared Error (RMSE):** Our final submission optimized for both accuracy and speed, achieved a competitive RMSE score placing us on 8th rank. 
- **Processing Speed:** We designed our solution to be run efficiently on Kaggle's GPU environment, meeting the competition’s speed requirements.

## File Structure 📂

```plaintext
.
├── Team_Matrix_updated.ipynb  # Solution Notebook
├── README.md                  # Project documentation
