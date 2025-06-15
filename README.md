# MSCS-634-M40_-KNN_RNN_Classification
Classification Using KNN and RNN Algorithms


# Wine Dataset Classification using KNN and RNN

This repository contains a Jupyter notebook that demonstrates the application of K-Nearest Neighbors (KNN) and Radius-Based Nearest Neighbors (RNN) classification algorithms on the Wine dataset.

## Overview

The Wine dataset is a classic machine learning dataset consisting of the results of a chemical analysis of wines grown in the same region in Italy but derived from three different cultivars. The analysis determined the quantities of 13 constituents found in each of the three types of wines.

## Dataset Information

- **Source**: UCI Machine Learning Repository
- **Instances**: 178 wine samples
- **Features**: 13 continuous attributes derived from chemical analysis
- **Classes**: 3 types of wine (class 0, 1, and 2)
- **Class Distribution**: 
  - Class 1: 71 instances
  - Class 0: 59 instances
  - Class 2: 48 instances

## Features

The 13 attributes in the Wine dataset include:
- Alcohol
- Malic acid
- Ash
- Alcalinity of ash
- Magnesium
- Total phenols
- Flavanoids
- Nonflavanoid phenols
- Proanthocyanins
- Color intensity
- Hue
- OD280/OD315 of diluted wines
- Proline

## Project Contents

The notebook [KNN_RNN_Classification.ipynb](KNN_RNN_Classification.ipynb) includes:

1. **Data Loading and Exploration**
   - Loading the Wine dataset
   - Examining the dataset structure
   - Displaying basic statistics and class distribution

2. **Data Preprocessing**
   - Splitting the data into training and testing sets (80/20 split)
   - Using stratified sampling to maintain class proportions

3. **KNN Implementation**
   - Training K-Nearest Neighbors classifiers with various k values (1, 5, 11, 15, 21)
   - Evaluating model performance with accuracy metrics
   - Visualizing the relationship between k values and accuracy

4. **RNN Implementation**
   - Training Radius-Based Nearest Neighbors classifiers with different radius values (350-600)
   - Evaluating model performance with accuracy metrics
   - Visualizing the relationship between radius values and accuracy

5. **Comparison and Analysis**
   - Comparing KNN and RNN performance
   - Discussing optimal parameter values
   - Analyzing when to use each algorithm

## Key Findings

- KNN achieves higher accuracy than RNN for this dataset
- Best KNN accuracy: 0.8056 with k=5 (and stable for larger k values)
- Best RNN accuracy: 0.7222 with radius=350
- KNN's accuracy is relatively stable for larger k values
- RNN's accuracy decreases as radius increases

## Usage

To run this project:

1. Clone this repository
2. Ensure you have the required dependencies installed:


pip install scikit-learn pandas matplotlib

3. Open the Jupyter notebook:


## Conclusions

This project demonstrates that KNN is preferable for the Wine dataset, as it achieves higher accuracy and is less sensitive to parameter changes. KNN works well when the data is well-clustered and classes are balanced, while RNN may be better suited for datasets with varying density or when explicit control over the influence region is needed.

## License

This project is available under the MIT License.
