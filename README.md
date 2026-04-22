# 🚢 Titanic Survival Prediction

This project builds and evaluates multiple machine learning models to predict whether a passenger survived the Titanic disaster using structured data.

## 📌 Overview

The goal of this project is to:

* Load and preprocess Titanic dataset
* Train multiple classification models
* Evaluate performance using key metrics
* Select and save the best-performing model
* Perform a sample prediction

---

## 📂 Dataset

The dataset used is:

```
train (2).csv
```

It should be located at:

```
/content/drive/MyDrive/train (2).csv
```

> ⚠️ Make sure your Google Drive is mounted if running in Google Colab.

---

## ⚙️ Features

* Handles missing values using median imputation
* Scales numeric features using standardization
* Uses pipeline architecture for clean ML workflow
* Compares multiple models:

  * Logistic Regression
  * Random Forest
  * Gradient Boosting
* Evaluates models using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
* Displays confusion matrix & classification report
* Saves the best model using `joblib`
* Performs a sample passenger prediction
* Visualizes model performance

---

## 🧠 Models Used

| Model               | Description                |
| ------------------- | -------------------------- |
| Logistic Regression | Baseline linear classifier |
| Random Forest       | Ensemble of decision trees |
| Gradient Boosting   | Boosted ensemble model     |

---

## 📊 Evaluation Metrics

Each model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Training Time

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/your-username/titanic-prediction.git
cd titanic-prediction
```

2. Install dependencies:

```bash
pip install pandas scikit-learn joblib matplotlib
```

3. Run the script:

```bash
python titanic_prediction.py
```

> If using Google Colab, ensure Google Drive is mounted.

---

## 💾 Output

* 📈 Model comparison table printed in console
* 🏆 Best model saved as:

```
best_titanic_model.pkl
```

* 📊 Bar chart comparing model performance
* 🔍 Sample prediction output

---

## 🔮 Sample Prediction

The model predicts survival for a sample passenger:

```python
{
    "Pclass": 3,
    "Sex": 1,
    "Age": 22,
    "SibSp": 1,
    "Parch": 0,
    "Fare": 7.25,
    "FamilySize": 1,
    "Embarked_C": 0,
    "Embarked_Q": 0,
    "Embarked_S": 1
}
```

---

## 📁 Project Structure

```
├── titanic_prediction.py
├── train (2).csv
├── best_titanic_model.pkl
└── README.md
```

---

## 🛠️ Future Improvements

* Add categorical encoding (e.g., one-hot encoding)
* Perform hyperparameter tuning
* Use cross-validation
* Deploy model as API (Flask / FastAPI)
* Add web interface

---

## 🤝 Contributing

Feel free to fork this repo and submit pull requests to improve the project.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## ✨ Acknowledgments

* Kaggle Titanic Dataset
* Scikit-learn library
