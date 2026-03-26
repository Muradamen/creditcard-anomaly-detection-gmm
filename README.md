

# 💳 Credit Card Fraud Detection using Gaussian Mixture Models (GMM)

🚀 ALX Data Science Portfolio Project
       #ALXProjectPortfolio

<img width="1408" height="768" alt="Anamolydetection" src="https://github.com/user-attachments/assets/ac60778e-8fba-42ac-8ecb-1b7f8850f0dd" />
## 🚨 Problem Statement

In modern financial systems, millions of transactions occur every day. Among them, a small fraction are fraudulent—but these rare events can lead to:

- 💸 Significant financial losses  
- 🔐 Security and privacy risks  
- 📉 Loss of customer trust  

Traditional fraud detection s
ystems rely heavily on **labeled data**, which is:

- Scarce and expensive to obtain  
- Highly imbalanced (fraud <1%)  
- Often outdated as fraud patterns evolve  

👉 **Key Challenge:**  
How can we detect fraudulent transactions **without relying on labeled data**?



## 💡 Solution

This project builds an **unsupervised anomaly detection system** using **Gaussian Mixture Models (GMM)**.

Instead of learning from labeled fraud examples, the model:

- Learns the **probability distribution of normal transactions**  
- Assigns a likelihood score to each transaction  
- Flags **low-probability transactions as anomalies (potential fraud)**  

## 🧠 Why Gaussian Mixture Models?

Gaussian Mixture Models are effective because they:

- Model complex data as a combination of multiple distributions  
- Capture hidden structures in high-dimensional data  
- Provide **probabilistic scoring**, ideal for anomaly detection  

## 🧰 Tech Stack

- **Python**
- **Pandas & NumPy**
- **Scikit-learn**
- **Matplotlib & Seaborn**
- **Jupyter Notebook**

## 📊 Dataset

- **Source:** [Credit Card Fraud Detection Dataset (Kaggle)  
](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
### Description
The dataset contains anonymized credit card transactions with:

- `Time` – Time elapsed between transactions  
- `Amount` – Transaction amount  
- `V1–V28` – PCA-transformed features  
- `Class` – Target label (0 = Normal, 1 = Fraud)  

### Key Characteristics

- ⚠️ Highly **imbalanced dataset**  
- Fraud cases represent **less than 1%**  
- Suitable for **unsupervised anomaly detection**

## 🔬 Methodology

### 1. Data Exploration
- Analyzed dataset structure and statistics  
- Investigated feature distributions  
- Identified severe class imbalance  


### 2. Data Preprocessing
- Scaled numerical features using `StandardScaler`  
- Prepared data for probabilistic modeling  

### 3. Model Development

- Implemented **Gaussian Mixture Model (GMM)**  
- Modeled the distribution of transaction data  
- Learned patterns of normal behavior  

### 4. Anomaly Detection Strategy

- Computed **log-likelihood scores** for each transaction  
- Defined a threshold for anomaly detection  
- Classified:
  - Low probability → 🚨 Fraud (Anomaly)  
  - High probability → ✅ Normal  

## 📈 Results & Evaluation

### 🔍 Key Insights

- Successfully identified **low-probability transactions as anomalies**  
- Demonstrated effectiveness of **unsupervised learning in fraud detection**  


### 📊 Performance Summary

- High **Recall** → Most fraud cases detected  
- Moderate **Precision** → Some false positives expected  
- Strong ability to separate normal vs anomalous transactions  


### 📉 Visual Analysis

The project includes visualizations such as:

- Class distribution (imbalance)  
- Log-likelihood score distribution  
- Anomaly detection patterns  


## 📂 Project Structure
creditcard-anomaly-detection-gmm/
│─ gmm_analysis.ipynb # Main analysis notebook
└── README.md


---
🚀 Future Improvements
Compare with:
Isolation Forest
Autoencoders
Optimize threshold selection using ROC analysis
Deploy as a real-time fraud detection API
Build a Streamlit dashboard

🎯 Key Takeaways
Unsupervised learning can solve real-world problems without labeled data
GMM provides a strong probabilistic approach to anomaly detection
Handling imbalanced datasets is critical in fraud detection

👨‍💻 Author

Murad Amin Imer
www.linkedin.com/in/muradamin

#ALXProjectPortfolio


## ▶️ How to Run the Project
### 1. Clone the repository
```bash
git clone https://github.com/Muradamen/creditcard-anomaly-detection-gmm.git
cd creditcard-anomaly-detection-gmm
pip install -r requirements.txt



