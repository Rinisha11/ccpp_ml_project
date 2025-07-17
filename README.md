
# Power Plant Energy Prediction

**Project Title:** Combined Cycle Power Plant Energy Output Prediction  
**Tech Stack:** Python · Scikit-learn · Pandas · Seaborn · Matplotlib  
**Notebook:** `CCPP_PowerPlant_Energy_Prediction.ipynb`  
**Dataset Source:** [UCI ML Repository - CCPP Dataset](https://archive.ics.uci.edu/ml/datasets/combined+cycle+power+plant) or Kaggle mirror

---

## Problem Statement

Predict the net hourly electrical energy output (PE) of a Combined Cycle Power Plant using environmental sensor data:  
- **Temperature (AT)**  
- **Exhaust Vacuum (V)**  
- **Ambient Pressure (AP)**  
- **Relative Humidity (RH)**  

The goal is to develop regression models that accurately predict PE based on these features.

---

## Dataset Overview

The dataset contains **9,568** data points collected from a power plant over **6 years**.

| Feature | Description |
|---------|-------------|
| AT      | Temperature (°C) |
| V       | Exhaust Vacuum (cm Hg) |
| AP      | Ambient Pressure (millibar) |
| RH      | Relative Humidity (%) |
| PE      | Net Energy Output (MW) - **Target Variable** |

---

## Project Workflow

1. **Import & Load Dataset**  
   `/kaggle/input/ccpp-energy-output/CCPP_data.csv`

2. **Exploratory Data Analysis (EDA)**  
   - Descriptive statistics  
   - Correlation matrix & heatmap  
   - Pairplots

3. **Data Preprocessing**  
   - Null check  
   - Train-test split (80/20)

4. **Model Training**  
   - Linear Regression  
   - Random Forest Regressor  

5. **Evaluation Metrics**  
   - R² Score  
   - Mean Squared Error (MSE)  

6. **Visualization**  
   - Actual vs Predicted PE comparison  
   - Model overlay scatter plot

---

## Model Performance

| Model              | R² Score | MSE     |
|--------------------|----------|---------|
| Linear Regression  | 0.930    | 20.27   |
| Random Forest      | 0.964    | 10.53   |

**Random Forest Regressor** performs better with lower error and higher accuracy.

---

## Visual Insight

![Model Predictions vs Actuals](./download.png)

---

## File Structure

\`\`\`bash
CCPP-Prediction/
 ┣ CCPP_PowerPlant_Energy_Prediction.ipynb
 ┣ download.png
 ┗ README.md
\`\`\`

---

## Future Work

- Add Polynomial Regression & XGBoost  
- Hyperparameter Tuning (GridSearchCV)  
- Deployment with Streamlit or Flask  
- Excel version comparison

---

## Author

**Rinisha Stanley**  
AI Enthusiast | Prompt Engineer | Data Storyteller  
[LinkedIn](https://www.linkedin.com/in/rinishastanley) | [GitHub](https://github.com/rinishastanley)
