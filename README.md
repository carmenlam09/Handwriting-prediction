# 🧠 Handwriting Prediction using Soft Computing

A hybrid **handwriting writer identification system** that integrates:
- Fuzzy Logic  
- Neural Networks (MLP & CNN)  
- Evolutionary Computing (Genetic Algorithms)  

Developed as part of **WIX3001 Soft Computing** coursework.

---

## 📌 Overview

This project identifies the **writer of handwritten characters** by combining multiple soft computing techniques:

- **Fuzzy Logic** → Handles uncertainty in handwriting  
- **Neural Networks** → Learns patterns from data  
- **Evolutionary Computing** → Optimizes model performance  

---

## 🚨 Problem Statement

Handwriting varies across individuals due to:
- Stroke thickness  
- Writing pressure  
- Slant and curves  

This project builds a system to:
- Identify writers from handwriting samples  
- Improve accuracy using hybrid AI techniques  
- Support applications like:
  - Signature verification  
  - Document authentication  
  - Forensic analysis  

---

## 📂 Dataset

- 5 writers (classes)  
- 720 handwritten samples  
- 144 samples per contributor  
- Processed into **28×28 grayscale images**

---

## ⚙️ Methodology

### 📝 Data Preprocessing

- Convert images to grayscale  
- Crop into segments  
- Resize to **28×28 pixels**  
- Center using bounding box  
- Convert to NumPy arrays  
- Label each image  

---

## 🧩 Model Architectures

### 🔹 Model 1: 

#### Fuzzy Logic (Feature Extraction)
Extracted features:
- Stroke thickness  
- Number of strokes  
- Line straightness  
- Loop size  

#### Neural Network (MLP)
- Dense layers
- Batch Normalization  
- Dropout 
- Softmax output

#### Evolutionary Computing
Optimized:
- Learning rate  
- Batch size  
- Epochs  
- Layers & neurons  
- Dropout rate
- Batch normalization  

---

### 🔹 Model 2: 

#### Fuzzy Logic (Image Enhancement)
- Enhances pixel intensity  
- Improves contrast  

#### Convolutional Neural Network (CNN)
- Conv2D
- MaxPooling 2D
- Flatten
- Dense layer
- Softmax output

#### Evolutionary Computing
Optimized:
- Learning rate  
- Filters  
- CNN layers  
- Dense neurons  

---

## 📊 Results

| Model | Before Optimization | After Optimization |
|------|------------------|------------------|
| Model 1 (MLP) | 0.4375 | 0.5208 |
| Model 2 (CNN) | 0.7083 | **0.75** |

✅ **Model 2 performs best**

---

## 🔍 Model Explainability

### Model 1
- LIME (Local Interpretable Model-agnostic Explanations)

### Model 2
- SHAP (SHapley Additive exPlanations)  
- Saliency Maps  

---

## 🧬 Evolutionary Computing

Genetic Algorithms used for hyperparameter tuning and performance optimization  

**Key Features:**
- Population-based search  
- Crossover & mutation  
- Fitness = model accuracy  

---

## 🏆 Key Findings

- CNN performs better for image data  
- Fuzzy logic improves preprocessing and feature extraction  
- Evolutionary computing boosts performance  

👉 **Best approach: Fuzzy + CNN + Genetic Algorithm**

---

## ⚖️ Model Comparison

| Aspect | Model 1 | Model 2 |
|------|--------|--------|
| Approach | Feature-based | Image-based |
| Neural Network | MLP | CNN |
| Accuracy | Lower | Higher |
| Complexity | High | Moderate |

---

## 🚀 Future Improvements

- Advanced fuzzy rules  
- Better optimization algorithms  
- Larger dataset  
- Reduce computational cost  

---

## 🛠️ Tech Stack

- Python  
- NumPy  
- Pandas  
- TensorFlow / Keras  
- scikit-learn  
- OpenCV  
- PIL (Pillow)  
- scikit-fuzzy  
- DEAP (Genetic Algorithm)  
- Matplotlib  
- LIME  
- SHAP  

---

## 👥 Contributors

- Tan Shun Qi  
- Carmen Lam Kah Man  
- Lee Zia Qian  
- Dernice Lee Tian Yi  
- Lim Shi Ting  

---

## 📄 License

This project is for academic purposes.
