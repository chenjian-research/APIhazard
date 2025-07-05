Overview

In this manuscript, we developed five common machine learning models, namely random forest, feedforward neural network, support vector regression, k-nearest neighbors, and extreme gradient boosting (XGBoost), to predict the pharmaceutical exceedance (i.e., mixture toxicity values exceeding 5% inhibition/lethality) for three representative trophic level species, including E. coli, R. subcapitata, and D. magna. The machine-learning models were implemented in Jupyter Notebook (V.7.0.8) using Python 3.12.

Hardware requirements

Only a standard modern computer is needed, with sufficient RAM to support in-memory processing of datasets.

Software requirements

These analyses are compatible with Windows, macOS, and Linux operating systems.

Installation Guide

Python is developed under an OSI-approved open-source license, making it freely usable and distributable. Python can be easy to pick up following the installation guide on the official website:
Installing Python: https://www.python.org/downloads/
Installing Jupyter: https://jupyter.org/install
Installing Python typically takes several minutes up to twenty minutes, depending on your internet connection and system setup.

Package dependencies:
After installing Python and Jupyter Notebook, you need install the following Python packages (if not already installed):
pip install scikit-learn, xgboost, shap, matplotlib, pandas, numpy, statsmodels, imblearn, geopandas
Installation may take approximately 10-20 minutes, depending on your internet speed and system specifications.

Running the demo:
We have provided a demonstration notebook (‘Demo_for_algae.ipynb’) and dataset files (‘Demo_algae.csv’ for training/testing and ‘Demo_predata.csv’ for prediction). These allow you to reproduce our results (Demo_for_algae.html) for predicting pharmaceutical exceedance in R. subcapitata in global rivers at a 2 km resolution using the XGBoost model.

Step-by-Step Instructions:
1. Model training and evaluation
In the first cell, you can load and run the code to input the training and test sets (‘Demo_algae.csv’). The code will train the XGBoost model and evaluate its performance using metrics such as accuracy, specificity, sensitivity, and AUC (area under the ROC curve).

2. Plot ROC curve
In the second cell, you can run the provided code to visualize the ROC curve and output the AUC value of the XGBoost model.

3. Threshold identification
In the third cell, you can execute the code to identify the threshold point where sensitivity equals specificity.

4. Feature importance
In the fourth cell, you can run the code to determine the relative contributions of each input feature. 

5. SHAP analysis
The fifth cell runs SHAP (SHapley Additive exPlanations) analysis to further interpret the model.

6. Prediction on riverine grid cells
In the sixth cell, you can input the prediction dataset (`Demo_predata.csv`) and run the code to predict pharmaceutical exceedance for R. subcapitata in 223,152 global riverine grid cells.

7. Global visualization
In the seventh cell, you can run the code to map the pharmaceutical exceedance for R. subcapitata in global rivers at 2 km resolution.

The outputs from this demo will match the results presented in our manuscript.

Support and Feedback
We welcome any questions, comments, or suggestions regarding the code, data, or analysis workflow. 

Thank you for your interest in our work!

Best wishes,

Jian (jianchen@hkbu.edu.hk)
