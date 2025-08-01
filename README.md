INCOME PREDICTION 

This project is about predicting whether someone makes over fifty thousand dollars a year using U.S. Census data. I used demographic features like age, education, occupation, marital status, and hours worked per week to train machine learning models that classify income level. The goal was to understand what types of models work best on this kind of data and how different preprocessing steps affect the results.

I started by cleaning the dataset, dropping rows with missing values, and applying one-hot encoding to the categorical features. I also normalized the continuous variables like age and hours per week so the models could learn better. After prepping the data, I trained and compared different classifiers including logistic regression, support vector machine, random forest, and XGBoost. I paid extra attention to class imbalance since most of the people in the dataset earn less than fifty thousand, and that could skew the results. To fix that, I used class weighting and looked at how the models performed on both classes separately.

XGBoost ended up performing the best in terms of overall accuracy and F1 score. I evaluated all the models using metrics like precision, recall, F1, and ROC AUC so I could get a more complete picture of performance. I also visualized feature importance and confusion matrices to see where the models struggled. Some of the most important features ended up being education level, occupation, and hours worked per week.

I also did a basic fairness check by looking at model performance across gender groups. I noticed some imbalance and want to look deeper into that next. The entire pipeline, from preprocessing to model evaluation, is in a single Jupyter notebook and works with the census dataset. You just need to make sure the csv file is in the same folder and run the cells in order. The project uses common Python libraries like pandas, scikit learn, matplotlib, and XGBoost.

This project helped me practice the full process of building a machine learning model from scratch, including data cleaning, model selection, evaluation, and interpretation. Everything in this repo was written and implemented by me.

