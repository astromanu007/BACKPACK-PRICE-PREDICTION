# 🎒✨ Backpack Price Prediction with Machine Learning

> 📈 Predict backpack prices with high accuracy using XGBoost and advanced feature engineering techniques.

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Model](https://img.shields.io/badge/Model-XGBoost-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

---

## 🧠 Project Overview

This project focuses on building a **machine learning pipeline** to **predict the retail price of backpacks** using a rich set of features like brand, material, compartments, waterproofing, and more. The project follows the full ML lifecycle:

🔍 EDA → 🛠️ Feature Engineering → 🧪 Model Training → 🚀 Submission

---

## 📦 Dataset Summary

| Dataset | Rows     | Columns | Description                  |
|---------|----------|---------|------------------------------|
| Train   | 300,000  | 11      | Includes `Price` (target)    |
| Test    | 200,000  | 10      | Predict `Price`              |

### 💡 Features include:
- 🏷️ `Brand`, `Material`, `Size`, `Color`
- 💻 `Laptop Compartment`
- 💧 `Waterproof`
- 📦 `Compartments`
- ⚖️ `Weight Capacity (kg)`
- 🎯 Target: `Price` (range: **$15 to $150**)

---

## 🧰 Tech Stack & Libraries

- 🐍 Python 3.x
- 📊 Pandas, NumPy, Seaborn, Matplotlib
- 🧪 Scikit-learn
- 🚀 XGBoost
- 🔍 Missingno (missing data viz)

---

## 🔬 Exploratory Data Analysis (EDA)

- 📉 Price distribution — nearly normal (Skewness ≈ 0.03)
- 📌 Missing values in multiple columns → handled with `'Unknown'` or mean
- 📊 Bar plots, boxplots, and distribution charts explored categorical effects

---

## ⚙️ Feature Engineering

✅ Handled missing values  
✅ One-hot encoding for categorical variables  
✅ Binned `Weight Capacity` into categories (`Light`, `Medium`, `Heavy`, etc.)  
✅ Scaled features using `StandardScaler`

---

## 🤖 Model: XGBoost Regressor

| Hyperparameter        | Value     |
|-----------------------|-----------|
| `n_estimators`        | 2000      |
| `max_depth`           | 8         |
| `learning_rate`       | 0.006     |
| `subsample`           | 0.7       |
| `colsample_bytree`    | 0.7       |

### 📊 Evaluation

- 📉 **RMSE (Validation Set)**: `38.96`
- 🔁 **5-Fold CV RMSE**: `39.11`

🎯 **Result**: Strong performance given the price range (15–150)

---

## 📁 Submission

✔️ Predictions generated on `test.csv`  
✔️ Final output saved as `submission.csv`

```csv
id,Price
1000001,47.89
1000002,91.23
...
````

---

## 🛠️ Future Enhancements

* 🔍 Hyperparameter tuning with **Optuna**
* 🤝 Model stacking or blending
* 🎯 Target encoding for high-cardinality categorical features
* 📦 Flask/FastAPI deployment for live price predictions

---

## 🧪 How to Run

```bash
# Clone the repo
git clone https://github.com/your-username/backpack-price-prediction.git
cd backpack-price-prediction

# Install dependencies
pip install -r requirements.txt

# Or run directly in Google Colab
# Upload `train.csv` and `test.csv`
# Open `backpacks_prediction.ipynb`
```

---

## 👨‍💻 Authors

* **Samarth Jadhav**
* **Manish Dhatrak**
* **Pawan Kudke**
* **Sakshi Fatangare**
* **Nisha Pavane**

📬 Contact: **[manishdhatrak1121@gmail.com](mailto:manishdhatrak1121@gmail.com)**

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🌟 Show Your Support

If you like this project:

⭐ Star it on GitHub
🍴 Fork it
📣 Share it with others!

> *"Prediction is very difficult, especially if it's about the future." — Niels Bohr*

````

---

### ✅ How to Use

1. **Copy & Paste** the above content into a new `README.md` file.
2. Replace `https://github.com/your-username/backpack-price-prediction.git` with your actual GitHub repo link.
3. Optional: Add screenshots or GIFs of plots/predictions for a more visual README.
4. Create a `requirements.txt` file with dependencies if you're planning to share this:

```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
missingno
````


