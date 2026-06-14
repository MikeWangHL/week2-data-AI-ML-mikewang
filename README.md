# week2-data-AI-ML-mikewang
Titanic Survival Prediction using a Decision Tree
week2-data-ml-mikewang

│
├── README.md
│
├── Titanic_Project.ipynb
│
└── screenshots
    └── decision_tree.png

## What the Project Does

This project uses a machine learning decision tree model to predict whether a passenger survived the Titanic disaster based on characteristics such as age, gender, ticket class, family size, and fare paid.

I chose this project because it is a well-known machine learning classification problem and provides a good introduction to data cleaning, predictive modelling, and model evaluation.

## How It Works

The dataset was first explored to identify missing values and understand the available variables.

The age variable contained missing values, which were replaced using the median age. The categorical variable "sex" was converted into numerical values so it could be used by the model.

The data was then split into training data (80%) and testing data (20%).

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

The Decision Tree model achieved an accuracy of approximately 79.9%.

The most influential variables were:

- Sex
- Passenger Class
- Age
- Fare

The model found that female passengers, younger passengers, and those travelling in higher classes generally had a greater chance of survival.

## What I Learned

This project helped me understand the complete machine learning workflow:

- Data exploration
- Data cleaning
- Feature preparation
- Model training
- Model evaluation

I also gained experience using Google Colab and GitHub for managing machine learning projects.

## Future Improvement

If I continued this project, I would compare multiple machine learning models such as Logistic Regression, Random Forests, and Gradient Boosting.

I would also explore additional feature engineering, such as creating family-size variables or using embarkation information to improve predictive performance.

Conclusion

The Decision Tree model achieved approximately 80% accuracy when predicting survival on unseen passengers.

The most influential predictors were sex, passenger class, age, and fare.

The model successfully identified patterns associated with survival and demonstrated how machine learning can use historical data to make predictions on new observations.
