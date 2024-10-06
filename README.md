# nyc-culinary-success-predictor
NYC Culinary Success Predictor: Developed a decision tree classifier to forecast restaurant performance in NYC based on key operational features

This repository contains the project “NYC Culinary Success Predictor”, developed to forecast restaurant performance in NYC using a decision tree classifier. The model analyzes key operational features to help restaurateurs make data-driven decisions, improving strategic planning and resource distribution.

Project Overview

In the highly competitive NYC restaurant industry, strategic decision-making is essential for success. This project provides restaurateurs with predictive insights based on restaurant ratings, neighborhood, cuisine type, and service quality. By analyzing these factors, the model forecasts restaurant performance and offers a blueprint for operational optimization.

Table of Contents

	•	Introduction
	•	Data Source
	•	Methodology
	•	Results
	•	Conclusion
	•	How to Use This Repository
	•	Requirements
	•	License
	•	Authors

Introduction

The NYC Culinary Success Predictor was designed to assist restaurateurs in making data-driven decisions by forecasting restaurant performance based on key operational features like food quality, service, location, and more. This project uses a decision tree classifier to predict ratings, aiming to enhance operational efficiency and customer satisfaction.

Data Source

We used the Kayak NYC Restaurant Directory as the main dataset, which contains approximately 1000 entries. The dataset includes information such as food quality, service, ambiance, restaurant ratings, and more. Categorical variables like cuisine and neighborhood were one-hot encoded, and ratings were categorized into low, medium, and high tiers.

Methodology

	1.	Data Preparation:
	•	Removed irrelevant columns such as ‘url’ and ‘reviews’.
	•	One-hot encoding was applied to categorical variables like cuisine, neighborhood, and price.
	•	Binned ratings (overall, food, service, ambiance) into three categories: low, medium, and high.
	2.	Modeling:
	•	Decision Tree Classifier: Initially, we built a fully grown tree to visualize the model. After tuning the hyperparameters using GridSearchCV, we achieved a balanced accuracy with minimal overfitting.
	•	K-Nearest Neighbors (KNN): Explored as an alternative model, the KNN classifier achieved an optimized accuracy of approximately 73.97% after parameter tuning.
	3.	Evaluation:
	•	The final decision tree model yielded a training accuracy of 90% and a testing accuracy of 91%. The model provided clear visualizations and feature importance measures to guide stakeholders in understanding the key factors driving restaurant success.

Results

	•	Top Predictors: Food quality emerged as the most significant factor in determining restaurant ratings, followed by service quality. Ambiance and cuisine type were less influential.
	•	Model Performance: The decision tree model showed strong generalization capabilities with minimal overfitting, and the ROC curve analysis indicated excellent sensitivity and specificity for predicting high and medium ratings.

Conclusion

The NYC Culinary Success Predictor offers restaurateurs a powerful tool for operational optimization. By focusing on key factors like food and service quality, restaurants can make informed decisions to improve customer satisfaction and business success.

How to Use This Repository

	1.	Data: The data/ folder contains the prepared dataset used for training the models.
	2.	Scripts: The scripts/ folder includes Python code for data preprocessing, model training, and evaluation.
	3.	Results: The results/ folder contains visualizations of the decision tree and evaluation metrics.
	4.	Report: The final project report is available in the docs/ folder.

Requirements

	•	Python 3.x
	•	Required libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

Install the required libraries by running:

pip install -r requirements.txt

License

This project is licensed under the MIT License - see the LICENSE file for details.

Authors

	•	Shu-Yu Hsu
	•	Tzu-Hsuan Lin
	•	Xuyan Zhang
