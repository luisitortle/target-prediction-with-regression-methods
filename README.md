"""# 
🏡 Housing Price Prediction with Regression Models  

This repository contains a Jupyter Notebook (`DATA PRACTICE.ipynb`) that explores **regression techniques** to predict housing **SALEPRICE** based on various property features. The work was developed as part of **Applied Physics 157 (THY - TX-2)**.  

---

## 📊 Dataset  
The project uses a dataset named `predict_home_value.csv`. Features include:  
- `ATSALEAGE` – Age of property at sale  
- `LOTAREA` – Lot size in square feet  
- `OVERALLCOND` – Overall condition rating  
- `YEARBUILT` – Year the house was built  
- `TOTRMSABVGRD` – Number of rooms above ground  
- `KITCHENABVGR` – Number of kitchens above ground  
- `FIREPLACES` – Number of fireplaces  
- `GARAGECARS` – Garage capacity  

**Target variable:**  
- `SALEPRICE`  

---

## 🧪 Methods  
The notebook implements and evaluates five regression methods:  
- **Huber Regressor**  
- **Kernel Ridge Regression**  
- **MLP Regressor (Perceptron)**  
- **Random Forest Regressor**  
- **AdaBoost Regressor**  

Each model is trained on 80% of the data and tested on 20%, with **feature scaling** applied where appropriate.  

---

## 📌 Results Summary  
| Regression Method        | Train R² | Test R² |  
|---------------------------|---------|--------|  
| Huber Regression          | ~0.646  | ~0.633  |  
| Kernel Ridge Regression   | ~-4.373 | ~-5.883 |  
| MLP Regressor             | ~-4.671 | ~-5.651 |  
| Random Forest Regression  | ~0.963  | ~0.717  |  
| AdaBoost Regressor        | ~0.703  | ~0.562  |  

**Key Insight:**  
- **Random Forest** achieved the best predictive performance.  
- **Huber Regression** was robust to outliers.  
- **Kernel Ridge** and **MLP** performed poorly on this dataset.  
- **AdaBoost** was decent but less effective than Random Forest.  

---

## ⚙️ Tools & Libraries  
- Python 3.x  
- Pandas, NumPy, Matplotlib  
- Scikit-learn (`HuberRegressor`, `KernelRidge`, `MLPRegressor`, `RandomForestRegressor`, `AdaBoostRegressor`)  

---
