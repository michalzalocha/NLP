# **NLP**

## **1. About project**
The goal of the project is to classify emotions in texts from social media.

---

## **2. Data**
**Source: Kaggle**  

**Link:**  
`https://www.kaggle.com/datasets/thedevastator/tweeteval-a-multi-task-classification-benchmark`  

**Description:**  
- number of samples:  3223
- number of columns:  2
- data type:  csv
- rodzaj of classes:  classes of emotions (anger, joy, sadness, optimism)

---

## **3. Goal**
Comparison of the effectiveness of three different text classification approaches in terms of emotion prediction quality.

The model assigns one of four emotions to a single tweet. The project reveals which model performs best with this type of data.

---

## **4. Models**

### **6.1 Classical ML**
- Algorithm: Logistic Regression
- Result: F1-macro: 0.52

### **4.2 Neuron network**
- Architecture: Dense
- Number of neurons: 4
- Result: F1-macro: 0.59

### **4.3 Transformer (fine-tuning)**
- Model name: distilBERT
- Used library: HuggingFace Transformers
- Result: F1-macro: 0.79

---

## **5. Ewaluacja**
**Metrics used: accuracy, precision, recall, F1‑score (macro)**  
**  

**Models comparison:**

| Model | Main metric | Result | Comments |
|--------|----------------|--------|--------|
| Classical ML | F1-macro | 0.52 |  |
| Neuron network | F1-macro | 0.59 |  |
| Transformer | F1-macro | 0.79 | best |

**Visualisation:**  
- Confusion matrix
- ROC curve

---


## **6. Structure**
```
project_NLP/
│
├── data/
│ ├── raw/
│ └── processed/
├── notebooks/
│ ├── 1_EDA.ipynb
│ ├── 2_Preprocessing_Features.ipynb
│ ├── 3_Models_Training.ipynb
│ └── 4_Evaluation.ipynb
├── models/
├── results/
├── README.md
└── requirements.txt
```
## **7. Technologies and libraries**
- Python 3.x  
- NumPy, Pandas, Matplotlib, Plotly, Seaborn, Joblib  
- scikit-learn  
- TensorFlow, PyTorch  
- HuggingFace Transformers  

---

Data source: https://www.kaggle.com/datasets/thedevastator/tweeteval-a-multi-task-classification-benchmark.

