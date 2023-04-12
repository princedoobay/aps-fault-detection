# Scania Air Pressure System Failure Prediction

This is an end-to-end machine learning project to predict failures in Scania's air pressure system using Python. The project includes data collection, preprocessing, exploratory data analysis, model building, selection, and deployment using Docker and AWS.

## Problem Statement

The air pressure system is a critical component in Scania's trucks. Failure of this system can lead to costly maintenance and downtime if it fails unexpectedly. The goal of this project is to build a machine learning model that can accurately predict failures and enable proactive maintenance, reducing downtime and minimizing maintenance costs.

## Data Collection

The dataset used in this project was provided by Scania and includes 58,000 samples, with 171 features and a binary target variable indicating whether a failure occurred.

## Data Preprocessing

The dataset had a large number of missing values, which required imputation. K-Nearest Neighbors imputation was used to fill in missing values. After preprocessing, exploratory data analysis was performed to gain insights into the data and visualize the relationship between features and the target variable.

## Model Building and Selection

Several machine learning models were built and trained to predict failures. The models included logistic regression, decision trees, random forests, and gradient boosting. Cross-validation and hyperparameter tuning techniques were used to optimize model performance. Performance was evaluated using metrics such as accuracy, precision, recall, F1 score, and AUC-ROC. The best-performing model was selected, which was a gradient boosting classifier.

## Deployment

After selecting the best-performing model, it was deployed using Docker and AWS. The application was containerized using Docker, which allowed the application to be run on different environments. Amazon SageMaker was used to train the model and create an endpoint to serve model predictions. The use of AWS ensured that the application is scalable, reliable, and can handle large volumes of traffic.

## Conclusion

This project showcases proficiency in data preprocessing, exploratory data analysis, machine learning, model selection, and deployment using Docker and AWS. By predicting failures in Scania's air pressure system ahead of time, this solution enables proactive maintenance, reduces downtime, and minimizes maintenance costs for Scania. 

## Requirements

- Python 3.x
- Pandas
- Numpy
- Scikit-learn
- Matplotlib
- Seaborn
- Flask
- Docker

## Usage

To use this project, follow these steps:

1. Clone the repository
2. Install the required libraries using `pip install -r requirements.txt`
3. Run the app using `python app.py`
4. Access the app at `http://localhost:5000` 

## Credits

This project was completed as a part of the machine learning course on Ineuron, and the dataset was provided by Scania.
