# China GDP Growth Analysis using Non-Linear Regression 📈🇨🇳

### 📌 **Overview**
This project explores the historical trajectory of China's GDP using **Non-Linear Regression**. While linear models often fail to capture the multi-phase nature of economic development, this project utilizes a **Sigmoid (Logistic) Function** to model the transition from slow developmental stages to rapid industrial growth. The model successfully fits the **"S-curve"** characteristic often seen in emerging economies.

---

### 📊 **Model Performance**
*   **Algorithm**: Non-Linear Regression (Sigmoid Model)
*   **Optimization Tool**: `scipy.optimize.curve_fit`
*   **Dataset Size**: 63 data points extracted from `china_gdp.csv`
*   **R-Squared Accuracy**: **0.7897**

---

### 💡 **Key Insights**
*   **Sigmoid Fitting**: The logistic growth model confirms that China’s economic expansion follows a distinct **"S-curve"**, showing a significant inflection point where growth accelerated exponentially before beginning to stabilize.
*   **Data Normalization**: Since GDP values and Years differ by several orders of magnitude, the model utilizes **Min-Max Scaling** (0 to 1) to ensure the regression algorithm converges efficiently.
*   **High Predictive Power**: An **R² of 0.79** indicates that the Sigmoid function is highly effective at capturing the non-linear dynamics of national economic growth compared to standard linear or low-degree polynomial models.

---

### 🛠️ **Tech Stack**
*   **Language**: Python 3.x
*   **Libraries**: `Pandas`, `NumPy`, `Scikit-Learn`, `Matplotlib`, `SciPy`
*   **Environment**: Google Colab

---

### 📁 **Repository Structure**
*   **`Non_Linear_Regression.ipynb`**: Full source code including automated "Brute Force" data cleaning and modeling.
*   **`china_gdp.csv`**: The historical dataset containing yearly GDP values.
*   **`Screenshot 2026-05-01 at 12.55.53 PM.jpg`**: Visualization of the actual data points versus the Sigmoid fit curve.

---

### 🚀 **Future Enhancements**
*   **Comparative Modeling**: Implementing Gompertz or Weibull functions to see if they offer a better fit for the later stages of economic maturity.
*   **Economic Forecasting**: Using the optimized **$\beta_1$** and **$\beta_2$** parameters to project potential GDP figures for the next decade.
*   **Multi-Country Analysis**: Applying this non-linear framework to other BRICS nations to compare industrialization speeds.

---
**Created by Shivi Srivastava as part of a Machine Learning portfolio project.**
