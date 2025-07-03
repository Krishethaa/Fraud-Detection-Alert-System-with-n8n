# Fraud-Detection-Alert-System-with-n8n

🚀 A machine learning powered system that detects fraudulent transactions and automatically sends fraud alerts via email using **n8n workflows**.

---

## 💡 Project Overview

This project combines:
- **Streamlit** for an interactive frontend where users can upload transaction data and view predictions.
- **A trained ML model (`model.pkl`)** to identify fraudulent transactions.
- **n8n** (open-source automation tool) to trigger fraud alert emails when frauds are detected.

---

## ⚙️ How It Works

1️⃣ Upload a CSV file of transactions using the Streamlit app.  
2️⃣ The app processes the file and highlights fraudulent transactions.  
3️⃣ For every fraud detected:
- The app sends data to an n8n webhook.
- n8n sends alert emails to the configured recipients.


---

## 🚀 How To Run Locally

 1️⃣ Run the Streamlit app
 -> streamlit run app.py

 2️⃣ Run n8n
You can run n8n via Docker:
 -> docker run -it -p 5678:5678 -v n8n_data:/home/node/.n8n n8nio/n8n
 
➡ n8n editor: http://localhost:5678
✅ Import projectDP.json into n8n to set up the workflow.
