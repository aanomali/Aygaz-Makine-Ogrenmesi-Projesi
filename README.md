# Crime Data Analysis with Supervised and Unsupervised Learning

This project analyzes crime data from 2020 to the present using both supervised and unsupervised machine learning techniques. The dataset used for this project is available from [Kaggle](https://www.kaggle.com/candacegostinski/crime-data-analysis).

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Supervised Learning](#supervised-learning)
- [Unsupervised Learning](#unsupervised-learning)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)

## Project Overview

This project focuses on crime data analysis using both supervised (Logistic Regression) and unsupervised (KMeans Clustering) learning algorithms. It includes data preprocessing, feature extraction, model training, and evaluation. The goal is to build models that can predict the status of crimes using supervised learning, and discover patterns and clusters of crimes using unsupervised learning techniques.

## Dataset

- **Dataset Name**: Crime Data from 2020 to Present
- **Source**: [Kaggle Crime Data](https://www.kaggle.com/candacegostinski/crime-data-analysis)
- **File Size**: 100+ MB
- **Features**:
  - `DR_NO`: Crime Record Number
  - `DATE OCC`: Date when the crime occurred
  - `Vict Age`: Victim's age
  - `Vict Sex`: Victim's gender
  - `LAT`, `LON`: Geolocation of the crime
  - `Crm Cd Desc`: Crime description
  - `Status`: Status of the crime (open/closed)
  - **Other features**: Crime type, location, etc.

## Technologies Used

- **Python**: Programming Language
- **pandas**: Data manipulation and analysis
- **matplotlib**: Data visualization
- **scikit-learn**: Machine learning models and preprocessing
- **Jupyter Notebook / VSCode**: IDE for code execution and development

## Project Structure

```plaintext
├── data/
│   ├── Crime_Data_from_2020_to_Present.csv  # Dataset file
├── crime_analysis.py                        # Main Python file for analysis
├── README.md                                # Project description
├── requirements.txt                         # Required libraries for the project
Installation
Step 1: Clone the Repository

git clone https://github.com/aanomali/Aygaz-Makine-Ogrenmesi-Projesi.git
cd Aygaz-Makine-Ogrenmesi-Projesi

Step 2: Install Dependencies
Make sure you have Python installed. Install the required libraries by running:

pip install -r requirements.txt
The requirements.txt file should include libraries like pandas, matplotlib, scikit-learn, etc.

Step 3: Run the Project
For supervised learning, Logistic Regression was used to predict the status of crimes (open/closed) based on available features like crime type, victim age, and geolocation.

Logistic Regression
Input Features: Categorical features (e.g., Crm Cd Desc, Vict Sex) are encoded using one-hot encoding. Numerical features like Vict Age are used directly.
Target Feature: Status
Performance Metric: Accuracy, Confusion Matrix, Classification Report
Result: Logistic Regression model accuracy: 85%
Unsupervised Learning
For unsupervised learning, KMeans Clustering was used to discover patterns and groups within the dataset.

KMeans Clustering
Input Features: Geolocation (LAT, LON), crime type, and other numerical attributes.
Clusters: 3 clusters were chosen for grouping the crimes.
Visualization: The clusters were plotted using latitude and longitude.

Model Evaluation
Confusion Matrix: To evaluate the performance of the Logistic Regression model, a confusion matrix was used.
Classification Report: Precision, recall, and F1-score were also calculated to assess the model.

Results:
Accuracy: 85%
Precision: 0.87
Recall: 0.82
F1-Score: 0.84

Conclusion
This project demonstrates the ability to predict crime status using supervised learning and find patterns in crime data using unsupervised learning. Logistic Regression performed well in classifying crime statuses, and KMeans was useful for clustering crime types based on geographical information.

