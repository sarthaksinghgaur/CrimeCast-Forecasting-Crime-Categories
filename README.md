# CrimeCast: Crime Category Prediction

CrimeCast is a machine learning project designed to predict the category of a crime incident based on structured data including time, location, modus operandi, and more. This project is implemented in a Jupyter Notebook (`.ipynb`) environment, focusing on real-world crime data preprocessing, feature engineering, model training, and evaluation.

---
## 🧠 Objective

To build a robust machine learning pipeline that predicts the category of a crime using various features such as date, time, location, and incident characteristics. The model can help law enforcement agencies with resource allocation and crime pattern analysis.

---

## 🔍 Features Used

* **Time\_Occurred**: Extracted features like hour, part of day
* **Date\_Occurred**: Extracted weekday, month, year
* **Location**: Categorical location info (hotspots, neighborhoods)
* **Modus Operandi**: Multi-label classification (converted to binary features)
* **Latitude & Longitude**: Used for mapping or clustering

---

## 🧹 Data Preprocessing

Performed inside `CrimeCast.ipynb`:

* Handled missing values
* Cleaned inconsistent entries
* Multi-label binarization (for Modus Operandi)
* One-hot encoding of categorical variables
* Feature scaling for numeric features

---

## ⚙️ Modeling

Several models were tested using scikit-learn:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* Gradient Boosting Classifier
* XGBoost Classifier

The best model was selected based on accuracy, F1 score, and cross-validation.

---

## 🏆 Final Model

* **Model Used**: RandomForestClassifier (with GridSearchCV)
* **Preprocessing**: Integrated using `Pipeline` and `ColumnTransformer`
* **Score Achieved**: \~0.95 weighted F1-score on validation data

---

## 🔧 Technologies Used

* Python
* Jupyter Notebook
* pandas, numpy, scikit-learn
* xgboost, matplotlib, seaborn

---

## 🚀 Running the Notebook

To execute the notebook:

1. Clone the repo:

```bash
git clone https://github.com/yourusername/CrimeCast.git
cd CrimeCast
```

2. Launch Jupyter:

```bash
jupyter notebook
```

3. Open `CrimeCast.ipynb` and run all cells

------

## 👨‍💼 Author

**Sarthak Singh Gaur**

---


## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

> Made with ❤️ using Jupyter Notebook & scikit-learn
