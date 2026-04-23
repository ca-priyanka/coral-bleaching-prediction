# DATA-207-Final-Project

Project Title: Coral Bleaching Classification and Prediction (Spring 2026)

Overview: For this project, we are interested in assessing coral bleaching through the application of various machine learning algorithms. We are focused on two key questions: (1) can we accurately classify images of bleached vs. healthy corals?, and (2) can we accurately predict the level of bleaching given a variety of other features such as water temperature and turbidity, coral depth, distance to shore, or global position (i.e., coordinates). 

👥 Team Members: Mackenzie Henderson, Marisa Aubert, Paola Piety and Priyanka Bhatnagar

## Repository Navigation

Repository includes: Exploratory data analysis (EDA), Data preprocessing and augmentation, Baseline and improved ML models 

Final notebooks:

    Enviromental Dataset (BCO):
        - BCO_Final_Preprocessing_EDA.ipynb
        - BCO_baseline_final_model.ipynb
        - BCO_FFNN_model.ipynb
        - BCO_HGB_model.ipynb
    
    Coral Image Dataset:
        - coral_images_preprocessing.ipynb
        - coral_images_EDA.ipynb
        - coral_images_baseline.ipynb
        - coral_images_improvement_model.ipynb

Individual notebooks: 

- Marisa's Notebooks: coral_images_preprocessing.ipynb, coral_images_baseline.ipynb, BCO_FFNN_model.ipynb
- Priyanka's Notebooks: BCO_Prep_EDA.ipynb, BCO_baseline_final_model.ipynb, coral_images_EDA.ipynb
- Mackenzie's Notebooks: BCO_Preprocessing.ipynb and coral_images_improvement_model.ipynb
- Paola's Notebooks: BCO_EDA.ipynb, BCO_Final_Preprocessing_EDA.ipynb and BCO_HGB_model


## Datasets and other details

📊 Datasets
1. BCO-DMO Global Bleaching & Environmental Dataset hosted by the Biological and Chemical Oceanography Data Management Office (BCO-DMO) compiles global coral bleaching observations from 1980 to 2020 with 62 different features such as site exposure, temperature, bleaching level, and more. The dataset contains 41,361 rows and 62 columns.
    Target variable: Risk level for coral bleaching (low, Medium, or High)

    Preprocessing steps include:

        Missing value handling

        Feature engineering

        Categorical encoding

        Train/validation/test split

2. Image Dataset: The Healthy and Bleached Corals Image Classification: ontains a total of 923 images of healthy (438) and bleached corals (485) collected from Flickr API. The images are in JPEG format with a maximum size of 300 pixels for width or height. The dataset is intended for training and evaluating image classification models to better assess coral reefs health, monitoring and contributing to their preservation or restoration.

    Preprocessing includes:

        Resizing

        Normalization

        Data augmentation (rotation, flips, brightness, etc.)

🔍 Exploratory Data Analysis (EDA)
Tabular EDA

    Distribution analysis

    Correlation heatmaps

    Feature importance (baseline models)

    Outlier detection

Image EDA

    Class balance visualization

    Sample image grids

    Augmentation previews

🤖 Modeling Approach
Tabular Models

    Baseline: Logistic Regression

    Improved models: Random Forest Classifier, Gradient Boosting or FFFN

    Evaluation metrics:

        Accuracy

        Log loss

        F1-score

Image Models

    Baseline: Logistic Regression

    Improved: Neural Network, CNN

    Evaluation metrics:

        Accuracy

        Confusion matrix

        Precision/recall


We follow a structured Git workflow:

    main — stable, production-ready code and documentation

    Feature branches:

        pri-image-eda

        m-auburt

        feature/[name]

Workflow:

    Create feature branch

    Commit work incrementally

    Open PR into main

    Merge into main after review