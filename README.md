# China GDP Growth Analysis using Non-Linear Regression 📈🇨🇳

### 📌 **Overview**
This project explores the historical trajectory of China's GDP using advanced modeling techniques. While traditional linear models often fail to capture complex economic shifts, this project compares a Sigmoid (Logistic) Function against a Multi-Layer Perceptron (MLP) Neural Network. The analysis demonstrates how increased model complexity can better capture the nuances of rapid industrial growth and stabilization in emerging economies.
---

### 📊 **Model Performance**
Based on the final project summary, the Neural Network approach provides a near-perfect fit compared to the mathematical Sigmoid baseline.
*   **Dataset Size**: 63 data points extracted from china_gdp.csv
*   **Sigmoid $R^2$ Accuracy**: 0.8183
*   **MLP Neural Net $R^2$**: 0.9904
*   **Mean Squared Error (MSE)**: 0.000823
*   **Neural Network Convergence**: Stopped at iteration 326
---

### 💡 **Key Insights**
*   **The Power of Complexity**: While the Sigmoid Model captures the general "S-curve" of growth, the MLP (Regularized) model (red dashed line in the plot) tracks the actual data points with significantly higher precision, achieving an $R^2$ of 0.99.
*   **Data Normalization**: The model utilizes Min-Max Scaling (0 to 1) for both GDP and Years. This is crucial for the Neural Network to achieve convergence within 326 iterations and maintain a low MSE.
*   **Inflection Points**: The visualization highlights that the MLP model better accounts for early-stage volatility and the specific curvature of China's economic acceleration compared to the more rigid Sigmoid baseline.
---

### 🛠️ **Tech Stack**
*   **Language**: Python 3.x
*   **Libraries**: `Pandas`, `NumPy`, `Scikit-Learn`, `Matplotlib`, `SciPy`
*   **Environment**: Google Colab

---

### 📁 **Repository Structure**
*   `Non_Linear_Regression.ipynb`: Full source code including automated "Brute Force" data cleaning and modeling.
*   `china_gdp.csv`: The historical dataset containing yearly GDP values.
*    '<img src="https://github.com/user-attachments/assets/5c186d6a-a65c-4be1-9b49-4d0d46cb4222" width="100%">'

**Figure 1:** Visualization of the actual data points versus the Sigmoid and MLP fits.Visualization of the actual data points versus the Sigmoid fit curve.

---

### 🚀 **Future Enhancements**
*   **Hyperparameter Tuning**: Experimenting with different hidden layer architectures in the MLP to maintain high accuracy while ensuring the model generalizes well to future data.
*   **Advanced Growth Functions**: Implementing Gompertz or Weibull functions as additional mathematical baselines to compare against the Sigmoid and MLP models.
*   **Economic Forecasting**: Leveraging the trained Neural Network (which achieved a $0.99$ $R^2$) to project potential GDP figures for the next decade.
*   **Multi-Country Analysis**: Applying this dual-model framework (Non-Linear Regression + Neural Networks) to other BRICS nations to compare industrialization speeds and model adaptability.

Created by Shivi Srivastava as part of a Machine Learning portfolio project.
