# 🧬 Genomics-Based Cancer Prediction Using Graph Attention Networks

This project explores the use of **Graph Attention Networks (GAT)** for predicting cancer types by integrating **multi-omics data** — specifically genomics, transcriptomics, and proteomics. It showcases a deep learning approach capable of capturing complex relationships in biological data, aiming to improve cancer classification accuracy.

---

## 📌 Overview

- 🔬 **Objective**: Predict cancer based on multi-omics data using a GAT model.
- 🧠 **Approach**: Graph-based learning enables the model to learn feature representations from a structured biological network.
- 🎯 **Accuracy Achieved**: Approximately **96%** on test samples (based on internal testing).

---

## 🧰 Technologies Used

- **Python**
- **PyTorch**
- **PyTorch Geometric**
- **pandas**
- **NumPy**
- **scikit-learn**
- **Jupyter Notebook**

---

## ⚠️ Important Note on Data

The actual datasets (`genomics.csv`, `transcriptomics.csv`, `proteomics.csv`) are **not included in this repository** due to size/privacy constraints.

> 🧪 You can adapt the code to any comparable omics dataset formatted as CSV files.  
> Each row should represent a patient/sample, and columns should represent gene/protein expression values.

---

## 📂 Project Structure

```plaintext
├── code.ipynb            # Jupyter notebook with full model pipeline
├── README.md             # Project overview and instructions
├── .gitignore
```

---

## 📊 Model Pipeline Summary

1. **Data Loading**  
   - Load genomics, transcriptomics, and proteomics data from CSVs.

2. **Preprocessing**  
   - Normalize data and encode class labels.

3. **Graph Construction**  
   - Each patient/sample is represented as a node.
   - Node features are derived from omics data.
   - Edges may be constructed based on biological similarity or defined manually.

4. **Graph Attention Network (GAT)**  
   - Train the model on the graph to classify cancer types.
   - Leverages attention mechanisms to prioritize informative nodes.

5. **Evaluation**  
   - Accuracy, loss tracking, and performance visualization.

---

## 🚀 How to Run

> Prerequisites: Python 3.8+, Jupyter Notebook, PyTorch, PyTorch Geometric

1. Clone the repository:
   ```bash
   git clone https://github.com/rudrikasharma15/genomics-based-Cancer-Prediction.git
   cd genomics-based-Cancer-Prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook code.ipynb
   ```

> ⚠ Replace the file paths with your own omics data CSVs.

---

## 📈 Results

The model demonstrates high predictive performance (~96% accuracy) on a multi-class cancer classification task using synthetic/internal datasets.

---

## 🔍 Future Work

- Add public datasets (or link to TCGA, GEO, etc.)
- Improve model generalization with cross-validation
- Expand to pan-cancer predictions with clinical metadata

---

## 📄 License

This project is licensed under the MIT License.  
Feel free to use or modify it for research and learning purposes.