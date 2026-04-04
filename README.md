# AIML 
 Student Career Prediction & Analysis
     
  Project Summary
 
 This project focuses on analyzing student data and predicting their future career paths based on various factors such as skills, interests, academic performance, and demographics.

The dataset contains information about 180 students, including:

Gender, Age, GPA
Interested Domain
Projects completed
Programming skills (Python, SQL, Java)
Future Career (target variable)

The project performs:
Exploratory Data Analysis (EDA) to understand patterns and distributions
Data preprocessing & encoding of categorical features
Visualization of relationships between skills, interests, and careers
Machine Learning / Deep Learning model to predict future careers
 Tools & Technologies Used
 Libraries
Pandas → Data manipulation & analysis
Matplotlib → Data visualization
Seaborn → Advanced visualization (heatmaps, barplots)
NumPy → Numerical operations
Scikit-learn → Preprocessing & train-test split
TensorFlow / Keras → Deep learning model
Techniques
Data Cleaning
Label Encoding
Feature Scaling (Normalization)
Data Visualization
Neural Network Modeling
             Project Workflow
1) Data Collection
Dataset loaded using pandas.read_csv()
2) Data Understanding
Checked:
.head() → Preview data
.info() → Data types
.describe() → Statistical summary
.isna() → Missing values
.duplicated() → Duplicate records
3) Data Cleaning
Removed unnecessary columns:
Student ID, Name, Major
Ensured no missing or duplicate data
4)Exploratory Data Analysis (EDA)

Performed multiple visualizations:

Gender distribution (Bar chart + Pie chart)
Interested domains distribution
Projects distribution
Skill distribution (Python, SQL, Java)
Age and GPA trends
Future career distribution

Advanced analysis:

Stacked Bar Chart → Career vs Interested Domain
Heatmap → Career vs Projects
Grouped Bar Chart → Skill comparison across languages
5️) Data Preprocessing
Converted categorical data using Label Encoding
Normalized numerical features using:
Mean and Standard Deviation scaling
6️) Model Building (Deep Learning)
Built a Neural Network using Keras Sequential API
Architecture:
Dense Layer (64 neurons, ReLU)
Dense Layer (64 neurons, ReLU)
Output Layer
7️) Model Training
Loss Function: Mean Squared Error (MSE)
Optimizer: RMSprop
Epochs: 130
Batch Size: 16
8️) Model Evaluation
Evaluated on test data:
Loss (MSE): ~0.031
MAE: ~0.0747
 Key Insights
Students with strong programming skills tend to align with technical careers
Domain interest strongly influences career choice
Certain projects are closely associated with specific career paths
Skill distribution varies significantly across languages
 Limitations
Label Encoding may introduce unintended ordinal relationships
Using MSE for classification is not ideal (should use categorical crossentropy)
Output layer should be adjusted for multi-class classification
 Future Improvements
Use Softmax activation with categorical crossentropy
Apply One-Hot Encoding instead of Label Encoding
Try advanced models:
Random Forest
XGBoost
Perform hyperparameter tuning
Deploy model using Flask or Streamlit

Conclusion

This project successfully demonstrates how student data can be analyzed and used to predict future careers using data science and deep learning techniques. It highlights the importance of skills, interests, and academic performance in shaping career paths.
