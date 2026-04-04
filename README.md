# AIML 
Student Career Prediction and Analysis
 Project Summary

This project analyzes student data to understand patterns and predict future career choices using machine learning techniques. The dataset consists of 180 student records containing demographic details, academic performance, technical skills, and career interests.

The main objective is to explore relationships between student attributes and their future careers, and to build a predictive model based on these features.

 Tools and Technologies
Libraries Used
Pandas for data manipulation
Matplotlib for basic visualizations
Seaborn for advanced visualizations
NumPy for numerical operations
Scikit-learn for preprocessing and data splitting
TensorFlow / Keras for building the neural network model
Techniques Applied
Data cleaning and preprocessing
Label encoding for categorical variables
Feature scaling (normalization)
Exploratory data analysis (EDA)
Deep learning model development

Project Workflow
   
1.1 Data Collection
The dataset was loaded using pandas from a CSV file

1.2 Data Understanding
Initial exploration was performed using:
head() for preview
info() for data types
describe() for statistical summary
isna() to check missing values
duplicated() to check duplicates

1.3 Data Cleaning
Removed unnecessary columns such as Student ID, Name, and Major
Confirmed that there were no missing or duplicate values

1.4 Exploratory Data Analysis
Several visualizations were created to understand the data:
Gender distribution using bar and pie charts
Distribution of interested domains
Analysis of student projects
Skill distribution in Python, SQL, and Java
Age and career distribution
Additional analysis included:
Stacked bar chart showing relationship between future career and domain
Heatmap showing relationship between future career and projects
Combined bar plots comparing programming skills

1.5 Data Preprocessing
All categorical variables were converted into numerical form using Label Encoding
Data was normalized using mean and standard deviation

1.6 Model Building
A neural network model was built using Keras Sequential API
The architecture included:
Two hidden layers with 64 neurons each and ReLU activation
One output layer

1.7 Model Training
Model was trained with:
Optimizer: RMSprop
Loss function: Mean Squared Error
Epochs: 130
Batch size: 16

1.8 Model Evaluation
The model was evaluated on test data
Performance metrics:
Loss (MSE): approximately 0.031
Mean Absolute Error (MAE): approximately 0.0747

 Key Observations
Students with stronger programming skills tend to move toward technical careers
Interested domain plays a major role in determining career choice
Specific projects are closely linked with certain career paths
Skill levels vary across different programming languages

 Limitations
Label encoding may introduce unintended relationships between categories
Mean Squared Error is not ideal for classification tasks
Output layer configuration is not optimized for multi-class classification

Future Improvements
Use Softmax activation with categorical crossentropy loss
Replace Label Encoding with One-Hot Encoding
Experiment with other models such as Random Forest or XGBoost
Perform hyperparameter tuning
Deploy the model using web frameworks

Conclusion

This project demonstrates how student data can be analyzed and used to predict future career paths. It shows the importance of combining data analysis with machine learning techniques to extract meaningful insights and build predictive systems.
