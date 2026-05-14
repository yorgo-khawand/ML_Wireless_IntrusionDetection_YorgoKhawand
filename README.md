# Wireless Intrusion Detection using Machine Learning

# Project Description
This project focuses on detecting wireless network intrusions using machine learning techniques.  
The AWID dataset was used as the main wireless traffic dataset. The original class labels in the dataset :

- '0' = Normal
- '1' = Injection
- '2' = Impersonation
- '3' = Flooding


Two machine learning models were implemented and compared:

- Decision Tree
- Random Forest

The goal of the project is to evaluate which model performs better for wireless intrusion detection based on common classification metrics such as Accuracy, Precision, Recall, F1-score, Balanced Accuracy, Confusion Matrix and ROC.

---

# Project Structure
ML_Wireless_ID_YorgoKhawand/
├── Report.docx
├── Demo_Video.mp4
├── README.md
└── Code/
    └── ML_model/
        ├── dataset/
        │   ├── AWID_CLS_R_Trn.csv
        │   └── AWID_CLS_R_Tst.csv
        ├── figures
        ├── dataset_preprocessing.py
        ├── train_model.py
        └── results_visualization.ipynb

# Setup Instructions

1. Download the Dataset

This project uses the AWID dataset.

Download it from:
https://www.kaggle.com/datasets/zhiqingcui/awidclsr/data (creating an account is required to download dataset)

After downloading:

Extract the files
Rename them to:
AWID_CLS_R_Trn.csv
AWID_CLS_R_Tst.csv

Move 2 files to the dataset folder.

2. Install Python

This project was developed using Python 3.13.7.

3. Install Required Libraries

Open terminal or command prompt and install:

pip install pandas numpy scikit-learn matplotlib jupyter.


4. Navigate to the project folder:
Start Jupyter Notebook using command:

jupyter notebook
or 
python -m notebook


Open:

results_visualization.ipynb

Run all cells from top to bottom.

5. (Optional) Run the training script from terminal instead of jupyter notebook 

Open terminal inside:
Code/ML_model/
Then run: 
python train_model.py  (will take couple of minutes)



# Tool Versions
Python: 3.13.7
Jupyter Notebook: 7.5.5
pandas: 3.0.2
numpy: 2.4.4
matplotlib: 3.10.8
scikit-learn: 1.8.0

# Expected Output

After running the code successfully, the project should produce:

1-Printed evaluation metrics for both models:
  Accuracy
  Precision
  Recall
  F1-score
  Balanced Accuracy
  Classification Report

2-A comparison table between:
 Decision Tree
 Random Forest

3-Output figures inside the figures/ folder and in notebook, such as:

confusion matrix for Decision Tree.
confusion matrix for Random Forest.
ROC for Decision Tree.
ROC for Random Forest.

4-A notebook showing the full workflow:

data loading
preprocessing
model training
evaluation
visualization
