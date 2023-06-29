## RealEstatePricePrediction
This project aims to predict real estate prices using the Boston Housing Dataset. Three machine learning models are employed in combination with a stacking technique. The final estimator used for stacking is Lasso regression. 

# Dataset
The dataset used for this project is the Boston Housing Dataset obtained from Kaggle. It consists of various features such as crime rate, property age, number of rooms, and more, which are used to predict the median value of owner-occupied homes in thousands of dollars.

# Models
The following models were utilized in this project:

AdaBoost: A boosting ensemble algorithm that combines multiple weak learners (decision trees in this case) to create a strong learner.

Gradient Boosting: Another boosting ensemble algorithm that sequentially trains decision trees to correct the errors made by the previous trees, resulting in an improved overall model.

XGBoost: An optimized implementation of gradient boosting that incorporates regularization techniques and parallel computing to enhance performance.

# Stacking
Stacking is a model ensemble technique that combines the predictions of multiple models as input to a final estimator. In this project, the predictions from AdaBoost, Gradient Boosting, and XGBoost models are stacked together, and Lasso regression is used as the final estimator to make the ultimate prediction.

# Usage
To run this project locally, follow these steps:

Clone this repository:
'''
git clone https://github.com/your-username/real-estate-price-prediction.git
'''

Install the required dependencies:
'''
pip install -r requirements.txt
'''
Execute the main script:
'''
python main.py
'''

# Results
The performance of the stacked model using Lasso regression as the final estimator was evaluated using various metrics such as mean squared error (MSE) and R-squared (R2) score. The results showed improved prediction accuracy compared to using individual models alone.

# Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.
