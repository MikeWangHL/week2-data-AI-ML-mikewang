# Titanic Survival Prediction Using a Decision Tree

**Week 2 AI & ML Mentorship Project**

Dataset: Titanic (Kaggle / Seaborn)

Model: Decision Tree Classifier

Accuracy: 79.9%

## Repository Structure

```text
week2-data-ml-mikewang
│
├── README.md
├── Titanic_Project.ipynb
└── screenshots
    └── decision_tree.png
```

## Project Objective

The goal of this project was to build a machine learning model capable of predicting passenger survival on the Titanic using demographic and travel-related information.

The project demonstrates the fundamental stages of a machine learning workflow, including data exploration, cleaning, model training, evaluation, and interpretation.

## What the Project Does

This project uses a machine learning decision tree model to predict whether a passenger survived the Titanic disaster based on characteristics such as age, gender, ticket class, family size, and fare paid.

I chose this project because it is a well-known machine learning classification problem and provides a good introduction to data cleaning, predictive modelling, and model evaluation.

## Dataset

This project uses the Titanic dataset, a widely used introductory machine learning dataset originally provided through Kaggle's "Titanic – Machine Learning from Disaster" competition.

The objective is to predict passenger survival using demographic and travel-related information.

## How It Works

The dataset was first explored to identify missing values and understand the available variables.

The age variable contained missing values, which were replaced using the median age. The categorical variable "sex" was converted into numerical values so it could be used by the model.

The data was then split into training data (80%) and testing data (20%).

A decision tree works by repeatedly splitting passengers into smaller groups based on characteristics that best separate survivors from non-survivors.

A Decision Tree Classifier was trained on the training data and used to predict survival outcomes on the test data.

The model achieved approximately 80% accuracy on unseen passengers.

## Tools Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- GitHub

## Challenge Encountered

While cleaning the data, I encountered a Pandas SettingWithCopyWarning when replacing missing values in the age variable.

Although the code worked correctly, the warning indicated that Pandas was unsure whether I was modifying a copy or a view of the original dataset.

After researching the issue, I learned that creating an explicit copy of the dataframe using .copy() would prevent the warning and make the operation safer.

This helped me better understand how Pandas handles dataframe slicing and assignment.

## Results

The Decision Tree model achieved an accuracy of approximately 79.9% on unseen test data.

This means the model correctly classified roughly 80 out of every 100 passengers whose outcomes it had not previously seen.

The most influential variables were:

| Feature | Importance |
|----------|------------|
| Sex | 0.606 |
| Passenger Class | 0.210 |
| Age | 0.075 |
| Fare | 0.061 |

The model found that female passengers, younger passengers, and those travelling in higher classes generally had a greater chance of survival.

## What I Learned

This project helped me understand the complete machine learning workflow:

- Data exploration
- Data cleaning
- Feature preparation
- Model training
- Model evaluation

I also learned that model performance depends heavily on data preparation, and that handling missing values correctly is an important part of the machine learning workflow.

## Future Improvement

If I continued this project, I would compare multiple machine learning models such as Logistic Regression, Random Forests, and Gradient Boosting.

I would also explore additional feature engineering, such as creating family-size variables or using embarkation information to improve predictive performance.

## Conclusion

This project provided a practical introduction to the end-to-end machine learning process, from data cleaning and feature preparation to model training and evaluation. The results demonstrated how a relatively simple model can identify meaningful patterns within historical data and make useful predictions on unseen observations.

## Decision Tree Visualisation
<img width="1317" height="631" alt="decision_tree" src="https://github.com/user-attachments/assets/82935f6f-87a4-470e-89af-37b9e03f51f5" />
