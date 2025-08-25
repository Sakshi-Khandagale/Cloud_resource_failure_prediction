# Cloud Task Failure Prediction ☁️⚡

## 📌 Business Problem

In cloud environments, tasks can either succeed or fail due to various reasons such as insufficient resources, high CPU usage, memory overload, or I/O bottlenecks. Task failure leads to downtime, wasted resources, and increased operational costs.

The objective of this project is to predict whether a cloud task will fail or not based on its system resource utilization, enabling proactive measures to reduce failures and improve reliability.

---

## 🎯 Objective

- Build a machine learning model to classify tasks as Failed or Successful.

- Perform data preprocessing: handling missing values, duplicates, and outliers.

- Apply feature engineering and train classification models.

- Evaluate performance using appropriate metrics (accuracy, precision, recall, F1-score).

---

## 📂 Dataset

Source: cloud_optimizer.csv

Features include:

- cpu_usage → CPU consumption level

- memory_usage → RAM utilization

- disk_io, network_io → I/O statistics

- task_status → Running / Waiting / Completed

- failure_flag (target variable) → Whether the task failed or not
  
---

## 🛠 Approach

1️⃣ Data Understanding & Cleaning

- Dropped irrelevant columns (vm_id, timestamp).

- Filled missing values (numerical → median, categorical → mode).

- Removed duplicates.

- Treated outliers using boxplots and statistical techniques.

2️⃣ Feature Engineering

- Encoded categorical variables.

- Normalized/standardized numerical features.

- Created target column for task failure prediction.

3️⃣ Model Building

Applied ML models such as:

- Logistic Regression

- Decision Trees

- Random Forest

- Support Vector Machine (SVM)

- Gradient Boosting 

- XGBoost

4️⃣ Model Evaluation

Used metrics like:

- Accuracy → Overall correctness

- Precision & Recall → Reliability in predicting failures

- F1-Score → Balance between precision and recall

- Confusion Matrix → Distribution of predicted vs actual results

---

## 📊 Results & Insights

- Identified key factors contributing to task failure (e.g., high CPU + memory spikes).

- Best performing model achieved high F1-score, showing strong balance in predicting both failed and successful tasks.

- Insights help in early detection of risky tasks, preventing downtime.

  ---

## 🧰 Tools & Libraries Used

- Python 🐍

- Pandas, NumPy → Data preprocessing

- Matplotlib, Seaborn → Visualization

- Scikit-learn, XGBoost → Machine Learning models

  ---
  

## ✅ Conclusion

The project demonstrates how machine learning can predict task failures in cloud systems. By analyzing resource usage and patterns, organizations can take proactive measures to reduce failures, improve system reliability, and optimize operational costs.


---


## 📌 Future Scope

- Implement real-time prediction system integrated with cloud monitoring.

- Use deep learning models (RNN, LSTM) for sequence-based prediction.

- Deploy as a dashboard for cloud admins to track task health in real-time.

---

## ✨ Developed by Sakshi Khandagale
