Heart Disease Prediction - Progress Evaluation I

1. Overview of the Project

    This project is part of the IT2011 - Artificial Intelligence & Machine Learning module.
    We selected the real-world problem: Predicting Heart Disease Risk using Machine Learning.

    The aim of Progress Evaluation I is to preprocess and analyze the dataset before applying machine learning models. Each team member contributes by applying one preprocessing technique. The final cleaned dataset will be used for model training in the next stage.

2. Dataset Details

    Name: Heart Disease Dataset
    Source: [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
    Size: 1,025 patient records
    Type: Tabular, structured

    Features (13):
        Age, Sex, Chest Pain Type, Resting BP, Cholesterol, Fasting Blood Sugar
        Resting ECG, Max Heart Rate, Exercise Angina, ST Depression, ST Slope
        Number of Major Vessels, Thalassemia
        Target Variable: heart_disease (1 = disease present, 0 = no disease)

3. Group Member Roles

    1.  IT24102753 - Indrajith A.G.T.           -   Preprocessing Technique 1 - Feature Scaling / Normalization	Applied StandardScaler and MinMaxScaler

    2.  IT24102739 - Kumarasinghe H.K.M.E.S.    -   Preprocessing Technique 2 - Feature Selection

    3.  IT24102748 - Wijerathna K.M.S.R.        -   Preprocessing Technique 3 - Feature Engineering - Dimensionality Reduction

    4.  IT24102775 - Damsana D.V.	            -   Preprocessing Technique 4 - Outlier Removal

    5.  IT24102697 - Jayawardhana D.D.S.	    -   Preprocessing Technique 5 - Data Transformation

    6.	IT24102706 - Priyadarshani G.P.S.D.     -   Preprocessing Technique 6 - Correlation Thresholding


4. How to Run the Code

i.  Open Google Colab and mount Google Drive:
        from google.colab import drive
        drive.mount('/content/drive')


ii. Set Project Path:
        PROJECT_PATH = "/content/drive/MyDrive/AI_ML_Group_Project"

iii.Run each member's Notebook 
        Input file: data/raw/heart.csv

        Each notebook will:
            Load the raw dataset
            Apply the assigned preprocessing step
            Save the processed file in data/processed/
            Save plots in results/eda_visualizations/

iv.Group Integration
        Finally, open and run group_pipeline.ipynb
        This integrates all preprocessing steps
        Output: outputs/heart_dataset_final.csv

5.  Output

    The output is a fully preprocessed dataset with:
        Missing values handled (already done in dataset)
        Encoding (already done in dataset)
        Feature Scaling
        Feature Selection
        Feature Engineering
        Outlier Removal
        Data Transformation
        Correlation Thresholding