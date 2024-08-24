
# Death Classification Model for Himalayan Expeditions

## Introduction

This repository contains the code and data for a machine learning project aimed at predicting the probability of death for climbers during expeditions in the Himalayas. The model is developed using historical data from 1905 to 2020, focusing on identifying key factors contributing to fatalities in this extreme environment.

## Objective

The primary objective of this project is to build a classification model that can predict whether a climber is likely to die during an expedition in the Himalayas. The model considers various features such as age, gender, peak difficulty, and season of the climb to estimate survival chances.

## Data

The model was developed using four CSV datasets, which are included in this repository:

1. **Deaths Dataset**: Information about individuals who died during expeditions, including details like peak name, date, time, citizenship, gender, age, oxygen use, summit status, and cause of death.

2. **Expeditions Dataset**: Data on various expeditions, including peak name, nationality, year, season, sponsors, leaders, and other expedition-related details.

3. **Peaks Dataset**: List of peaks with their heights, whether they have been climbed, and information about the first ascent.

4. **Summiters Dataset**: Details about individuals who summited, including name, season of climb, date, time, citizenship, gender, age, oxygen use, and if they died on the descent.

## Project Structure

The repository is structured as follows:

- **data/**: This folder contains the CSV files used in the project.
- **notebook.ipynb**: The Jupyter notebook containing the full implementation of the classification model, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation.

## Dependencies

The project requires the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- imbalanced-learn
- scipy


## Usage

1. **Data Loading**: The notebook loads and preprocesses the data, handling missing values, feature encoding, and data merging.

2. **Exploratory Data Analysis (EDA)**: Graphical analysis of the data to understand distributions and relationships between different features.

3. **Feature Engineering**: Creation of new features such as "Climb Count" and binary encoding of categorical variables.

4. **Model Training and Evaluation**: Various machine learning models (K-Nearest Neighbors, Logistic Regression, Random Forest, SVM, Decision Tree) are trained and evaluated using metrics like accuracy, precision, recall, F1 score, ROC-AUC, and PR-AUC.

5. **Model Selection**: The RandomForestClassifier was selected as the best model based on its performance metrics, particularly in handling the imbalanced nature of the dataset.

## Results

The final model achieved a high degree of accuracy and robustness, making it a useful tool for predicting the risk of death during Himalayan expeditions. However, it's important to note the inherent unpredictability of such extreme environments, and the model's predictions should be used as one of many tools in expedition planning.

## Conclusion

While the model offers valuable insights into the factors influencing climber fatalities, it is not a definitive predictor of outcomes. The risk of death in the Himalayas is influenced by numerous unpredictable factors, and climbers should always prepare thoroughly and consult experts before embarking on expeditions.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Data sourced from [Kaggle](https://www.kaggle.com/datasets/raskoshik/himalayan-expeditions/data). Special thanks to the contributors who made this dataset available for public use.

