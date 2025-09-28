# 🏠 House Price Prediction using Linear Regression

## 📌 Overview
This project demonstrates a simple yet effective linear regression model to predict house sale prices based on key features such as living area, number of bedrooms, and bathrooms.  
It is built using Python and popular data science libraries, and is intended for internship applications and portfolio presentation.

---

## 📊 Dataset
- *Source:* Kaggle – Ames Housing Dataset  
- *Total Samples:* 1460  
- *Selected Features:*
  - GrLivArea: Above-ground living area (in square feet)
  - BedroomAbvGr: Number of bedrooms above ground
  - FullBath: Number of full bathrooms
- *Target Variable:* SalePrice (in USD)

---

## 🧮 Model Summary
- *Model Used:* Linear Regression
- *Train/Test Split:* 80/20 → 1168 training samples, 292 test samples
- *Intercept:* 94,203.09  
- *Coefficients:*
  - FullBath: +30,014.32  
  - GrLivArea: +104.03  
  - BedroomAbvGr: −26,655.17

### 📈 Evaluation Metrics
- *Root Mean Squared Error (RMSE):* $52,975.72  
- *R² Score:* 0.6341

---

## 📈 Visualizations

### 🔹 Actual vs Predicted Prices
![Actual vs Predicted](outputs/actual_vs_predicted.png)  
This scatter plot compares predicted house prices with actual sale prices.  
The red dashed line represents perfect prediction. Most points are clustered near the line, indicating decent model accuracy.

### 🔹 Residuals Distribution
![Residuals](outputs/residuals.png)  
This histogram shows the distribution of residuals (prediction errors).  
The curve is roughly centered around zero, suggesting that the model does not have strong bias and errors are symmetrically distributed.

---

## 💡 Key Insights
- The model captures general pricing trends well, especially with GrLivArea and FullBath.
- Negative coefficient for BedroomAbvGr may reflect quality-related factors or multicollinearity.
- RMSE of ~$53K is acceptable for a basic model, but further improvements are possible.

---

## 🚀 How to Run

1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/house-price-linear-regression.git
cd house-price-linear-regression

2. Install dependencies
`bash
pip install -r requirements.txt
`

3. Run the notebook
Open HousePriceLinear_Regression.ipynb in Jupyter Notebook and run all cells.

---

📦 Project Structure

house-price-linear-regression/
├── data/
│   └── train.csv
├── outputs/
│   ├── actualvspredicted.png
│   ├── residuals.png
│   ├── coefficients.csv
│   ├── metrics.csv
├── HousePriceLinear_Regression.ipynb
├── requirements.txt
├── README.md 

🙋‍♂ Author
Yash  
Aspiring machine learning practitioner and web developer  
Connect with me on LinkedIn or check out my GitHub