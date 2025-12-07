Project Overview
This project focuses on building an end-to-end explainable machine learning platform to predict hospital readmission risk while providing clear and interpretable insights for clinical use. The goal is not only to achieve accurate predictions but also to help healthcare professionals understand why a patient is classified as high or low risk. The entire workflow covers everything from raw clinical data processing to model prediction, explainability, and visualization through an interactive Power BI dashboard.

🧠 Machine Learning Model
For the prediction task, I developed a Random Forest classifier to handle multi-class readmission risk prediction. Since real hospital data usually suffers from class imbalance, class-weight balancing was applied to improve fairness in predictions. The dataset was split using an 80–20 train–test strategy, and model performance was evaluated using accuracy, precision, recall, F1-score, and the confusion matrix to ensure reliable results.

🔍 Explainability Layer (XAI)
To make the model suitable for clinical decision-making, several explainability techniques were implemented. Global feature importance was used to identify the most influential factors contributing to readmission risk. Accumulated Local Effects (ALE) plots helped explain how the predicted risk changes with variations in important features. PDP and ICE plots were also generated to visually interpret the overall and patient-level model behavior.

📊 Power BI Dashboard
An interactive Power BI dashboard was created to visualize both predictions and explainability results in a user-friendly manner. The dashboard displays feature importance, high-risk patient percentages compared with targets, risk trends based on time spent in the hospital, and specialty-wise risk analysis. It also includes age group-based risk distribution and interactive slicers for age group and medical specialty to allow dynamic exploration.

🏗️ System Architecture
The system follows a structured pipeline where raw CSV-based clinical data is first ingested and then cleaned using preprocessing steps such as encoding, normalization, and feature engineering. This processed data is passed into the Random Forest model for prediction, followed by the explainability layer using feature importance and ALE. Finally, all results are visualized using Power BI dashboards for decision support.

🛠️ Tech Stack
The project was developed using Python with key libraries such as Pandas, NumPy, Scikit-learn, and Matplotlib. Jupyter Notebook was used as the main development environment. Power BI was used for building interactive dashboards, and explainability was handled using feature importance, ALE, PDP, and ICE techniques.

🎯 Project Objective
The main objective of this project is to design a transparent, accurate, and clinician-friendly machine learning system that not only predicts hospital readmission risk but also explains model decisions clearly and visualizes healthcare patterns in an interactive way.

👨‍⚕️ Applications
This platform can be used for hospital readmission monitoring, clinical risk assessment, healthcare operations optimization, and as a decision-support system for doctors and hospital administrators.

🚀 Future Enhancements
In the future, this system can be enhanced by integrating SHAP-based patient-level explanations, connecting with real-time EMR systems, enabling real-time prediction using streaming data, applying AutoML for hyperparameter tuning, and deploying the platform as a web application using Flask or FastAPI.

👩‍🎓 Academic Context
This project was developed as part of my Master’s in Computer Science with a focus on Explainable AI, Healthcare Analytics, Clinical Machine Learning Systems, and Visual Decision-Support Platforms.
