# 📈 Financial Time-Series Forecasting with RNNs
[![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-Keras%20%2F%20TensorFlow-orange.svg)](https://tensorflow.org)
[![Pandas](https://img.shields.io/badge/Library-Pandas%20%2F%20NumPy-red.svg)](https://pandas.pydata.org)

## 📌 Project Overview
This project focuses on building and evaluating **Deep Learning** architectures to predict financial indicators using historical Yahoo Stock Price data (2015–2020). The primary goal was to move beyond simple regression and implement **Recurrent Neural Networks (RNNs)** capable of handling sequential dependencies in market data.

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Deep Learning:** Keras, TensorFlow (RNN & LSTM layers)
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib (FiveThirtyEight style)
* **Optimization:** Adam Optimizer, MSE Loss Functions

## 🚀 Key Milestones
1.  **Data Exploration & Validation:** Analyzed 1,825 unique daily records. Conducted data integrity checks (null handling, date unique-indexing).
2.  **Stationarity Evaluation:** Assessed the statistical properties of the time series to determine the stability of the mean and variance.
3.  **Model Selection:** Developed and benchmarked various RNN-based architectures.
4.  **Future Forecasting:** Visualized the "Predicted vs. Actual" values to determine the effective predictive horizon of the model.

## 📊 Performance Insights
* **Accuracy Horizon:** The model demonstrates high reliability for short-term forecasts (up to 2 time-steps).
* **Error Analysis:** Successfully identified "linear behavior" bias in the initial RNN results, where the model maintained a constant slope.
* **Scalability:** The architecture was designed to be modular, allowing the same logic to be extrapolated across all four market indicators (High, Low, Open, Close).

## 💡 Engineering Reflection (The "Honest" Breakdown)
In the spirit of technical transparency, this project includes a critical self-evaluation section:
* **The Challenge:** Identified that standard RNNs can struggle with non-linearity without proper regularization.
* **The Solution:** Proposed a hybrid approach combining **Lasso/Ridge Regression** with Time-Series Forecasting to improve feature correlation and prevent overfitting.
* **Conclusion:** While the current model serves as a strong learning framework, it highlights the necessity of **Dropout layers** and **Regularization** for real-world economic deployments.

## 📂 Project Structure
```text
├── data/
│   └── yahoo_stock.csv        # 5 years of historical financial data
├── notebooks/
│   └── time-series-forecasting.ipynb  # Main analysis and model pipeline
└── README.md                  # Project documentation
📬 Contact
LinkedIn: [[Your Profile Link](https://www.linkedin.com/in/vandana-sharma-20a5ab24a/)]

