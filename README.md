##  End to End Machine Learning Project

## 1. Create Virtual Environment: Virtual Environment for separate projects

2. Create Requirements.txt file: To install libraries (e.g., numpy, pandas)

3. Create setup.py file: Whenever we want to convert the whole project into the packages

4. Creating notebooks folder: Inside the notebook folder, we should create a data folder for uploading a dataset. This notebook folder will not convert into the package, it's just for to do our EDA purpose.

(i) Data Folder

(ii) Data.csv (inside Data folder)

(iii) EDA.ipynb

(iv) Model Training.ipynb

5. Creating a source folder: My entire machine learning life cycle should be run inside this source folder. Whenever we create a folder, we should always create an init.py file. Because this source folder is also a package, we should be able to reuse it and install it somewhere else.
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

6. Artifacts folder - This folder will create by code not manually, this folder is for saving our outputs.

7. Logs - To saving the log details and this folder will create by code not manually.

8. app.py - To create a web application for our model

9. templates folder

(i) index.html

(ii) form.html

10. Dockerfile - To deploy in the cloud.


# Salary Prediction
