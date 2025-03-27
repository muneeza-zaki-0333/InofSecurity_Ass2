🚨 Malicious URL Classification

An end-to-end pipeline for detecting and classifying malicious URLs into the following five categories:

✅ Benign

🧠 Defacement

🎣 Phishing

💀 Malware

📩 Spam




Malicious Url Classification
🚨 Malicious URL Classification
An end-to-end pipeline for detecting and classifying malicious URLs into the following five categories:

✅ Benign

🧠 Defacement

🎣 Phishing

💀 Malware

📩 Spam

This repository includes robust Python code for:

📁 Repository Structure
malicious-url-classification/
├── data/                 # Folder for input CSV datasets
├── notebooks/            # Jupyter notebooks for experiments
├── scripts/              # Python scripts for pipeline stages
├── models/               # Trained models and checkpoints
├── results/              # Metrics, visualizations, confusion matrices
├── requirements.txt      # Required dependencies
└── README.md             # Project documentation
🚀 Getting Started
✅ Prerequisites
Python 3.7+

pip or conda

GPU (optional) for LSTM/BERT-based training

📦 Installation
git clone https://github.com/<your-username>/malicious-url-classification.git
cd malicious-url-classification
Using pip:

pip install -r requirements.txt
Using conda:

conda create -n maliciousurl python=3.9
conda activate maliciousurl
pip install -r requirements.txt
📂 Data Files
Place your CSV datasets in the data/ folder:

benign.csv

defacement.csv

malware.csv

phishing.csv

spam.csv

Update paths in scripts if using custom filenames or directories.

🧱 Pipeline Components
1. 📊 Data Merging
Combine all class-based CSVs into a single dataset

2. 🧹 Preprocessing
Handle missing values

Remove duplicates

Detect and treat outliers

Encode class labels (e.g., label encoding)

3. ⚖️ Balancing
Use SMOTE or class-weight strategies to fix class imbalance

4. 📈 Exploratory Data Analysis (EDA)
Descriptive statistics

At least 5 visualizations:

URL length distributions

Class balance

Character distributions

Word cloud by class

TF-IDF heatmaps

5. 🔍 Feature Extraction
Structural features: URL length, number of special characters, entropy, etc.

NLP features:

TF-IDF vectors

Word2Vec embeddings

Character-level n-grams

Transformer embeddings (BERT, GPT-style)

🤖 Model Training
Implement and train multiple models:

🎲 Random Forest

📈 Support Vector Machine (SVM)

⚡ XGBoost

🔁 LSTM (sequence-based)

🧠 CNN

🤖 Fine-tuned BERT / GPT models

📊 Results Visualization
Confusion Matrix

ROC Curves

Accuracy / Precision / Recall Comparison Plots

🏁 Performance & Results
Structural + NLP features boost performance

Fine-tuned BERT achieved ~89.1% accuracy

Traditional models (e.g., XGBoost) performed well (~87.5%)

🧩 Challenges & Future Improvements
URL obfuscation and adversarial generation

Real-time classification support

Incremental learning / streaming URLs

Lightweight deployment (ONNX, TF Lite)

🤝 Contributing
PRs are welcome! Please open an issue or submit a pull request for bug fixes or feature additions.

📜 License
Distributed under the MIT License. See LICENSE for details.

🏁 Conclusion
This project demonstrates a powerful and flexible pipeline for URL threat classification using both classical ML and advanced transformer-based approaches. With proper tuning and feature engineering, this pipeline can be adapted to real-world cybersecurity applications.

Built with ❤️ and security in mind.
