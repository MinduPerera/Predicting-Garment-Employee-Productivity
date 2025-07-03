# 🎯 Final Report: Predicting Garment Employee Productivity

## 📌 Objective
To predict the actual productivity of sewing operators using available operational data.

---

## 🔧 Models Compared
| Model Code | Model                 | R² Score | RMSE     |
|------------|-----------------------|----------|----------|
| RF         | Random Forest         | **0.383** | **0.0154** |
| XGB        | XGBoost               | 0.330    | 0.0167   |
| LR         | Linear Regression     | 0.307    | 0.0173   |
| Poly       | Polynomial Regression | 0.285    | 0.0179   |

---

## 📈 Performance Visualization
![image](https://github.com/user-attachments/assets/e3888181-f2b7-4a59-937b-23d9694328e2)


---

## 🧠 Insights
- Removing `target_productivity` reduces R² for all models.
- Random Forest still performed best, indicating its ability to generalize and capture patterns from other features.
- Features such as `smv`, `wip`, `no_of_workers`, and `over_time` contribute meaningfully to predictions.

---

## ✅ Conclusion
Even without access to targets, ML models can still provide useful productivity estimates. Random Forest is a strong choice for deployment in planning tools to improve efficiency and reduce reliance on over-time.

---

## 💾 Next Steps
- Hyperparameter tuning (especially for XGBoost)
- Aggregate features by date/team for group-level forecasting
- Deploy model using Streamlit for planners to use easily

