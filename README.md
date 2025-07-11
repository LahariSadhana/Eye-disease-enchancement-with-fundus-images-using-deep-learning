# 🩺 Eye Disease Detection with Explainable AI (VGG16 + LIME + SHAP)

This project leverages deep learning (VGG16) to classify **8 eye disease categories** from retinal fundus images. To enhance model interpretability, it integrates **LIME** and **SHAP** explanations into a **Streamlit-based web app** for intuitive user experience.

## 📌 Project Goals

- Predict eye diseases from fundus images using a VGG16-based CNN.
- Visualize predictions using **LIME (Local Interpretable Model-agnostic Explanations)**.
- Create a **Streamlit GUI** for easy user interaction and file upload.
- Highlight explainability for **transparent AI diagnosis**.

---

## 🧠 Model Summary (VGG16 Fine-tuned)

- **Base Model:** VGG16 (imagenet weights, frozen layers)
- **Added Layers:**
  - Dense(2048, relu) + Dropout(0.4)
  - Dense(2048, relu) + Dropout(0.4)
  - Dense(8, softmax) for 8 classes
- **Metrics:** Accuracy, Confusion Matrix, F1-Score

## 📁 Disease Classes

- Normal
- Cataract
- Diabetes
- Glaucoma
- Hypertension
- Myopia
- Age-related Macular Degeneration
- Other Abnormalities



## 🖥️ Streamlit GUI Features

- Upload JPG/PNG fundus image
- Real-time prediction
- LIME explanation with boundary map
- Clean UI with sidebar uploader
