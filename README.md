# SafeEdgeNER  

### Named Entity Recognition for Security and Defense  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Hugging Face](https://img.shields.io/badge/HuggingFace-Transformers-yellow) ![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML%20Tools-orange) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)  

## 📌 Description  

**SafeEdgeNER** is an academic **Named Entity Recognition (NER)** project applied to the security and defense domain. The goal is to automatically identify relevant entities such as military platforms, weapons, locations, temporal references, and official documents in large amounts of unstructured textual data.  

The system uses advanced **Deep Learning** models, including **BERT** and **RoBERTa**, to ensure high accuracy in entity extraction.  

## 🚀 Technologies Used  

- **Python**  
- **Hugging Face Transformers**  
- **PyTorch**  
- **Scikit-learn**  
- **Pandas & NumPy**  
- **Matplotlib & Seaborn** (for result analysis)  

## 📂 Project Structure  

```bash
SafeEdgeNER/               
│── documents/                
│── notebooks/             # Jupyter notebooks
│   │── EDA.ipynb               
│   │── NER_BERT.ipynb
│   │── NER_CRF.ipynb
│   │── NER_RoBERTa_test1.ipynb
│   │── NER_RoBERTa_test2.ipynb
│   │── NER_RoBERTa_test3.ipynb
│   │── NER_RoBERTa_test4.ipynb
│   │── NER_RoBERTa_test5.ipynb
│   │── NER_RoBERTa_test6.ipynb
│   │── NER_RoBERTa_test7.ipynb
│── README.md             
│── LICENSE                # Project license
```

## 📊 Dataset  

The project uses a dataset adapted from the **re3d** corpus, which includes documents related to conflicts in Syria and Iraq. The dataset has been preprocessed and converted into the **CoNLL 2003 IOB2** format for proper entity annotation.  

The main recognized entities are:  
- **Location** (e.g., cities, geographic coordinates)  
- **MilitaryPlatform** (e.g., ships, tanks, aircraft)  
- **Weapon** (e.g., AK-47, missiles)  
- **Temporal** (e.g., dates, times)  
- **DocumentReference** (e.g., official document identifiers)  
- **Person** (names of individuals)  
- **Organisation** (e.g., governments, military groups)  
- **Money** (currencies, amounts of money)  

## 🔧 Usage  
you can run the notebooks on **Google Colab** by uploading them to a Colab workspace and running the cells.

### **1️⃣ Exploratory Data Analysis (EDA)**  
To analyze the dataset, use:  
```bash
jupyter notebook notebooks/EDA.ipynb
```

### **2️⃣ Train Models**  
Various models were tested, including BERT, CRF, and RoBERTa. To run a specific training notebook, use:  
```bash
jupyter notebook notebooks/NER_BERT.ipynb   # For BERT model training
jupyter notebook notebooks/NER_CRF.ipynb    # For CRF model training
jupyter notebook notebooks/NER_RoBERTa_test5.ipynb  # For RoBERTa model training 
```
Additional RoBERTa training attempts are available in the other numbered notebooks.  

## 📈 Results  

Tests on models showed that **RoBERTa** achieved the best performance in entity recognition, with an **average F1-score of 0.88** and an **accuracy of 89%**.  

### Optimizations  

Several **optimization** techniques were applied to improve performance of our RoBERTa model, including:  
✔️ **Data Augmentation** (Synonym Augmentation, Contextual Embedding Augmentation)  
✔️ **Class Weights** to handle class imbalance  
✔️ **Focal Loss** to reduce the impact of more frequent classes  
✔️ **Increased number of epochs** to enhance training  

## 👥 Contributors  

The project was developed by:  
- **Micol Zazzarini**  
- **Andrea Fiorani**  
- **Antonio Antonini**    

## 📜 License  

This project is distributed under the **MIT** license. See the `LICENSE` file for more details.  

---  



