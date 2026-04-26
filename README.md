# Automated Kidney Lesion Classification with Explainable AI

An end-to-end AI-driven clinical decision support system for automated kidney lesion classification from CT images. This project addresses key challenges in medical imaging such as variability in radiologist interpretation, subtle lesion detection, and lack of explainability in traditional deep learning models.

The system leverages multiple CNN architectures (Custom CNN, MobileNetV2, EfficientNetB0, and ResNet50) with transfer learning to perform multi-class classification (Normal, Cyst, Stone, Tumor). A comparative analysis identified **ResNet50 as the best-performing model (~81% accuracy)** with strong precision-recall balance, making it suitable for real-world healthcare scenarios.

To enhance trust and interpretability, **Grad-CAM explainability** is integrated to highlight clinically relevant regions in CT scans. The system also introduces **confidence-based risk stratification**, automated **diagnostic report generation**, and an **AI-powered assistant**, making it a complete intelligent healthcare solution rather than just a prediction model.

📌 *Published in IJEDR (Impact Factor: 9.37)*

---

## 🌟 Key Features

- 🧠 Deep Learning Model using **ResNet50 (~81% accuracy)**
- 🔍 **Grad-CAM Explainability** for visual interpretation
- ⚠️ **Confidence-Based Risk Prediction** (Low / Medium / High risk)
- 📄 Automated **PDF Diagnostic Report Generation**
- 🤖 AI-powered **Clinical Assistant (Chatbot)**
- 🖥️ Interactive UI for **real-time CT image upload & prediction**
- 📊 Model comparison across **4 architectures**

---

## 📂 Modules

- **Prediction Module**  
  Classifies CT images into Normal, Cyst, Stone, Tumor with confidence scores  

- **Explainability Module**  
  Generates Grad-CAM heatmaps highlighting important regions  

- **Risk Assessment Module**  
  Converts confidence scores into actionable clinical risk levels  

- **Reporting Module**  
  Generates structured downloadable diagnostic reports  

- **AI Assistant Module**  
  Provides medical insights, precautions, and guidance (support tool)

---

## 🧪 Model Architecture & Approach

- Compared 4 models:
  - Custom CNN (baseline)
  - MobileNetV2
  - EfficientNetB0
  - **ResNet50 (Best Performer)**

- Used **Transfer Learning + Fine-Tuning**
- Image preprocessing:
  - Resizing (224x224)
  - Normalization
  - Data augmentation (rotation, zoom, flip)
- Evaluation Metrics:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix

---

## 📊 Results

- ✅ ResNet50 achieved ~**81% accuracy**
- 📈 Better generalization compared to other models
- 🔍 Grad-CAM highlights matched **clinically relevant kidney regions**
- ⚠️ Confidence-based system helps identify **uncertain cases**
- 📄 End-to-end pipeline: **Prediction → Explanation → Risk → Report**

---

## 📁 Dataset

- CT Kidney Dataset (~5,700 images)
- Classes:
  - Normal
  - Cyst
  - Stone
  - Tumor

## 📊 Dataset  
This project uses the publicly available CT Kidney Dataset from Kaggle:  
[📊 CT Kidney Dataset (Normal, Cyst, Tumor, Stone)](https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone)

---

## 🛠️ Technologies Used

- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy  
- Pandas  
- Matplotlib  

---

## ⚠️ Disclaimer

This system is designed as a **decision-support tool** and not a replacement for medical professionals. Predictions should always be reviewed by qualified clinicians.

---

## 📄 Documentation  
[📄 View Project Documentation (PDF)](KidneyLesionDocumentation.pdf)

## 📄 Research Paper  
[📄 View Research Paper (IJEDR – IF: 9.37)](ResearchPaper.pdf)

