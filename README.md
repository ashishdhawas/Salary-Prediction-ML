# Salary Prediction

The project seeks to build a robust predictive model that accurately estimates salaries based on demographic attributes, contributing valuable insights to the understanding of income disparities and the complex interplay of factors that influence earnings within diverse demographic contexts.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction

The focus of the Demographic-Based Salary Prediction project is to develop a predictive model that estimates the salaries of individuals from diverse countries and races based on their demographic attributes. These attributes encompass a range of variables, including occupation, age, gender, experience, and education. The dataset for this project, acquired from Kaggle with 7 independent variables and the target variable, "Salary."

## Dataset

The dataset provides an expansive compilation of salary and demographic information, augmented by details regarding years of professional experience. It serves as a valuable resource for investigating the intricate relationship between income and various socio-demographic factors. Demographic features such as age, gender, education level, country of origin, and race constitute the foundation for a comprehensive analysis. This dataset empowers researchers to uncover patterns and trends in income distribution across diverse demographic categories, shedding light on potential variations or inequalities in earning potential. Additionally, the dataset incorporates a crucial dimension - "Years of Experience" - offering a lens into the impact of accumulated professional tenure on salary levels. This dynamic facet enables in-depth exploration of how income is influenced by both demographic attributes and the evolution of professional expertise. Overall, the dataset presents an opportunity for conducting exhaustive studies on income diversity and gaining insights into the multifaceted determinants that shape earning prospects in today's workforce.

## Methodology

1. **Data Preprocessing:** Cleaning the dataset, handling missing values, and converting categorical variables into numerical representations.

2. **Exploratory Data Analysis (EDA):** Exploring the data to understand distributions, correlations, and potential patterns between independent features and dependent feature.

3. **Feature Engineering:** Creating new features or transformations that might enhance the predictive power of the model.

4. **Modeling:** Building and training machine learning models to predict salary of the employee. Experimenting with regression algorithms such as Linear Regression, Random Forest, and Gradient Boosting.

## Exploratory Data Analysis

During the EDA phase, we conducted various analyses, including:

- Distribution of independent features and salary.
- Correlations between different features and salary.
- Visualization of key features' impact on salary.

## Feature Engineering

Based on our EDA, we engineered some features categories because we have so many number of categories we combined similar categories.

## Modeling

We used various regression algorithms to train our model on the dataset. The models were evaluated using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) score to assess predictive performance.

## Results

Our best-performing model achieved an R-squared score of 94 %, indicating its ability to accurately predict salary of the employee. The most influential features for salary prediction were found to be [list_top_features_here].

## Conclusion

Predicting salary is a complex task due to the interplay of multiple factors. This project demonstrates that machine learning models can provide valuable insights into employee salary. However, further refinement and fine-tuning are necessary to achieve even more accurate predictions.

## Usage

To replicate or build upon this project:

1. Clone this repository.
2. Download the dataset from kaggle and place it in the `data` directory.
3. Use Jupyter Notebook or your preferred environment to run the analysis and modeling scripts.

## Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request to this repository.

##  End to End Machine Learning Project

#### 1. Create Virtual Environment: Virtual Environment for separate projects

#### 2. Create Requirements.txt file: To install libraries (e.g., numpy, pandas)

#### 3. Create setup.py file: Whenever we want to convert the whole project into the packages

#### 4. Creating notebooks folder: Inside the notebook folder, we should create a data folder for uploading a dataset. This notebook folder will not convert into the package, it's just for to do our EDA purpose.

(i) Data Folder

(ii) Data.csv (inside Data folder)

(iii) EDA.ipynb

(iv) Model Training.ipynb

#### 5. Creating a source folder: My entire machine learning life cycle should be run inside this source folder. Whenever we create a folder, we should always create an init.py file. Because this source folder is also a package, we should be able to reuse it and install it somewhere else.
We should create the below files and folders inside the source file.

(i) __init__.py - To convert this folder into a package

(ii) exception.py - To handle the exceptions

(iii) logger.py - To create a log file

(iv) utils.py - utils.py file basically means any generic functionality probably that I want to create for this entire project.

(v) Components Folder

(vi) __init__.py file (inside components folder) - To convert this component folder into a package

(vi) data_ingestion.py file (inside components folder) - To extract the dataset from databases or somewhere else

(vi) data_transformation.py file (inside components folder) - To do feature engineering

(vii) model_trainer.py file (inside components folder) - To create a model

(ix) Pipeline Folder (inside source folder) - This folder is for training the model and predicting the model prediction.

(x) training_pipeline.py file (inside pipeline folder) - evaluating the model

(xi) predict_pipeline.py file (inside pipeline folder) - predicting for test data or new data

#### 6. Artifacts folder - This folder will create by code not manually, this folder is for saving our outputs.

#### 7. Logs - To saving the log details and this folder will create by code not manually.

#### 8. app.py - To create a web application for our model

#### 9. templates folder

(i) index.html

(ii) form.html

#### 10. Dockerfile - To deploy in the cloud.

1. Docker Build checked
2. Github Workflow
3. Iam User In AWS

## Docker Setup In EC2 commands to be Executed

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## Configure EC2 as self-hosted runner:

## Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app
