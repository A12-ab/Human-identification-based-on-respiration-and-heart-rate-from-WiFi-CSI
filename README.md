# Human Identification Using WiFi CSI Based on Respiration and Heart Rate

## 📌 Overview
This project focuses on **non-intrusive human identification** using **WiFi Channel State Information (CSI)** signals. It leverages both **respiration rate** and **heart rate** extracted from CSI data to uniquely identify individuals without requiring wearable devices. The approach applies **Machine Learning (ML)** and **Deep Learning (DL)** models with different fusion techniques for classification.

---

## 📂 Repository Structure
- `grand_final_preprocessing.ipynb` – CSI data preprocessing (noise removal, filtering, signal extraction).  
- `grand_final_feature_extraction.ipynb` – Extracts time-domain and frequency-domain features from processed signals.  
- `grand_final_ml_early.ipynb` – Implements ML models (SVM, Random Forest, KNN, Logistic Regression) with early fusion.  
- `grand_final_dl_early.ipynb` – Implements DL models (CNN, LSTM, BiLSTM) with early fusion for improved accuracy.  

---

## ⚙️ Features Extracted
- **Time-Domain:** Mean, Standard Deviation, Min, Max, Peak-to-Peak, Energy, Median, 25th and 75th Percentiles  
- **Frequency-Domain:** Dominant Frequency, Spectral Entropy  

---

## 🚀 Methodology
1. **Data Collection:** CSI data collected for multiple individuals using Atheros CSI Tool.  
2. **Preprocessing:** Noise filtering and isolation of respiration and heart rate signals.  
3. **Feature Extraction:** Combined time-domain and frequency-domain features.  
4. **Fusion Techniques:** Early Fusion (ML and DL), Weighted and Late Fusion (tested in ML).  
5. **Modeling:** Applied ML and DL classifiers to identify individuals.  
6. **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, Confusion Matrix.  

---

## 📊 Results
- **Best Performing Model:** LSTM with Early Fusion  
- **Performance:** Achieved the highest accuracy and F1-score compared to other models.  

---

▶️## Usage
1. Run grand_final_preprocessing.ipynb for data preprocessing.

2. Run grand_final_feature_extraction.ipynb for feature extraction.

3. Train ML models with grand_final_ml_early.ipynb.

4. Train DL models with grand_final_dl_early.ipynb.

5. Evaluate results using generated confusion matrix and performance metrics.

##📌 Applications
. Smart home security and access control

. Healthcare monitoring and patient identification

. Elderly care centers and fall detection systems

## 🛠️ Requirements
- Python 3.8+  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

Install dependencies:
```bash
pip install -r requirements.txt



##📜 License
This project is licensed under the MIT License.
