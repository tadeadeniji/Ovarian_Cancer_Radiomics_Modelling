# Ovarian_Cancer_Radiomics_Modelling
This repository contains files of python code that I used during my Internship in summer 2023 at the Department of Radiology, University of Cambridge, in the group Radiogenomics and Quantitative Image Analysis (led by Dr Lorena Escudero Sanchez)

- In this project, I tried to reproduce in Python and/or improve the results published in: 
L. Rundo, L. Beer, L. Escudero Sanchez et al., Clinically Interpretable Radiomics-Based Prediction of Histopathologic Response to Neoadjuvant Chemotherapy in High-Grade Serous Ovarian Carcinoma, Front. Oncol. 12 (2022) doi: 10.3389/fonc.2022.868265
https://www.frontiersin.org/journals/oncology/articles/10.3389/fonc.2022.868265/full
- The Radiomics features had been previously extracted and pre-selected.
- The Data used was from one external test set and one discovery (train) set. Each set contained subsets of CT scan radiomics features and results of NACT treatment (effective or not effective)
- Random Forest Classification is a machine learning technique used for categorizing data. It combines multiple decision trees, each built using a random subset of training data and features, to make a more robust prediction. The final classification is determined by taking a majority vote from all individual trees.
- The core concept is to develop a predictive model based on CT scan features that can accurately determine the efficacy of neoadjuvant chemotherapy (NACT) applied to patients with Ovarian Cancer. If successful, this model could facilitate personalized treatment plans, allowing some patients to bypass NACT when it's unlikely to be effective, thereby conserving resources and potentially saving lives.
- To start, Notebook 1 shows the use of Gridsearch in order to perform hyperparameter tuning. This is also visually displayed using heatmaps and the top 5 models are selected.
- Then, Notebook 2 is where we select the most appropriate model out of the top 5. We evaluate the models based on the discovery data set and different metrics such as Accuracy, sensitivity, and specificity.
- To end, Notebook 3 is where we evaluate these metrics further by creating insightful graphics, such as confusion matrices and ROC curves. This helps us conclude the effectiveness and robustness of the model.
