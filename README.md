
# Credit Card Fraud Detection

This project implements a machine learning pipeline to detect fraudulent credit card transactions using the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) from Kaggle.

---

## Dataset

- **Source:** [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- **Size:** 284,807 transactions  
- **Class distribution:** Highly imbalanced — only 492 fraud cases (~0.17%)  

---

## Project Overview

The goal is to accurately identify fraudulent transactions through the following steps:

1. **Data Exploration & Visualization**  
   Analyze feature distributions and class imbalance.

2. **Preprocessing**  
   Scale numerical features (`Amount` and `Time`) using StandardScaler.

3. **Data Balancing**  
   Apply SMOTE (Synthetic Minority Over-sampling Technique) to the training set to address class imbalance.

4. **Model Training**  
   Train an XGBoost classifier on the balanced dataset.

5. **Evaluation**  
   Evaluate model performance with confusion matrix, classification report, and ROC AUC score.

6. **Feature Importance**  
   Visualize the most important features contributing to fraud detection.

7. **Model Persistence**  
   Save the trained model for future inference.

---

## Installation

Make sure you have Python 3.7+ installed.  
Clone this repository and install the dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

### Run in Jupyter Notebook (optional)

Open and run the `creditcard_fraud.ipynb` notebook to explore the data and model training steps interactively.

### Run Streamlit App (optional)

To run a simple interactive app (if available), execute:

```bash
streamlit run app.py
```

---

## File Structure

```
.
├── creditcard.csv           # Dataset (download separately from Kaggle)
├── creditcard_fraud.ipynb   # Jupyter notebook (optional)
├── app.py                   # Streamlit app (optional)
├── model/                   # Folder for saved models
│   └── xgb_model.pkl
├── requirements.txt         # Python dependencies
└── README.md                # This file
```

---

## Notes

- The dataset is **not** included in the repository due to size constraints.  
- Download the dataset manually from Kaggle [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and place `creditcard.csv` in the project root.

---

## 🚀 Live Demo

Click the link below to try the live Streamlit app:

👉 [Open the App in Streamlit](https://fraudsense-credit-card-fraud-detection-dvufdydff9dp92mgfoadkx.streamlit.app/)


---


## Author

Leila Ghasemzadeh

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
