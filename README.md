#  Heart Disease Risk Prediction using Bayesian Networks

Welcome to **MediMystery Labs**, where you're the Data Detective! In this project, we use **Bayesian Networks** to predict the risk of heart disease based on patient data.

---

##  Project Overview

This project demonstrates:
- Cleaning and preprocessing real-world-style health data (`heart_disease.csv`)
- Applying **Min-Max scaling** and **discretization**
- Building a **Bayesian Network** using `pgmpy` with a predefined structure
- Training the network with **Maximum Likelihood Estimation**
- Performing **inference queries** to estimate heart disease risk
- Visualizing **network structure**, **CPDs**, and **inference results**

---

##  Dataset

Simulated patient data: [`heart_disease.csv`](https://bit.ly/3T1A7Rs)  
Contains fields such as:
- `age`
- `fbs` (fasting blood sugar)
- `target` (1 = heart disease, 0 = no disease)
- `chol` (cholesterol)
- `thalach` (max heart rate)

---

##  Setup Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/heart-disease-bayes.git
   cd heart-disease-bayes

2.Install the required libraries:

    pip install pandas scikit-learn pgmpy matplotlib networkx

3.Run the script or Jupyter Notebook:

---

<h3>📊 1. Bayesian Network Structure</h3>
<img src="Outputs_and_Graphs/BayesianStructure.png" alt="Bayesian Network" width="500"/>

<h3>📈 2. CPDs of Key Variables</h3>

<p><strong>🔹 Target</strong></p>
<img src="Outputs_and_Graphs/Graphs/cpd_for_target.png" alt="CPD - Target" width="400"/>

<p><strong>🔹 Cholesterol</strong></p>
<img src="Outputs_and_Graphs/Graphs/cpd_for_chol.png" alt="CPD - Chol" width="400"/>

<p><strong>🔹 Thalach</strong></p>
<img src="Outputs_and_Graphs/Graphs/cpd_for_thalach.png" alt="CPD - Thalach" width="400"/>

<p><strong>🔹 FBS</strong></p>
<img src="Outputs_and_Graphs/Graphs/cpd_for_fbs.png" alt="CPD - FBS" width="400"/>

<h3>🎯 3. Inference Result: P(target | fbs=2, age=1)</h3>
<img src="Outputs_and_Graphs/op1_with_graph.png" alt="Inference Result" width="500"/>