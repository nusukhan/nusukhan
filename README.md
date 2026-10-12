<h1 align="center">Hi, I'm Nusrat Anwar 👋</h1>
<h3 align="center">AI / ML Engineer</h3>

<p align="center">
I build systems that answer from real data, measure whether they got it right, and can name what they get wrong.
</p>

<p align="center">
  <a href="https://nusukhan.github.io">🌐 Portfolio</a> ·
  <a href="https://www.linkedin.com/in/nusrat-anwar-b5b836251">💼 LinkedIn</a> ·
  <a href="mailto:nusratanwar000@gmail.com">✉️ Email</a>
</p>

---

## 👩‍💻 About Me

I'm an AI/ML engineer based in Pakistan, available for work (remote or on-site). My focus is the full lifecycle of a model — cleaning and engineering the data, training and evaluating the model, and deploying it so people can actually use it.

A model that *runs* is not the same as a model that *works*. Across every project below the method is the same: build it, measure it against a held-out set, compare it to a baseline, and report what the measurement actually said — including the limitation I found while looking for it.

- 🔭 Seven projects, each one evaluated
- 🚀 Two deployed as a live app or API
- 📊 Spanning RAG, imbalanced classification, regression, object detection, computer vision and medical imaging
- 📫 Reach me at **nusratanwar000@gmail.com**

---

## 🛠️ Tech Stack

**Languages & ML**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=for-the-badge&logoColor=white)

**NLP & Vision**
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=for-the-badge&logo=spacy&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logoColor=black)

**Data & Tools**
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 🚀 Featured Projects

### 🧠 RAG Knowledge Extraction System — *flagship*
A hallucination-resistant Retrieval-Augmented Generation system that answers only from a corpus of 5,000 Wikipedia science articles, and reports how much of each answer its sources actually support. Built over 12 weeks, one stage per week — ingest, index, retrieve, generate, verify, serve.
**Retrieval accuracy 97% · ~2 ms retrieval · tested FastAPI service (6/6 tests, 5/5 concurrent)**
`Python` `ChromaDB` `sentence-transformers` `spaCy` `FastAPI` `pytest`
🔗 **[View repo →](https://github.com/nusukhan/parallax-week1)**

---

### 🛡️ Real-Time Credit Card Fraud Detection
Fraud is 0.17% of this dataset — a model that flags nothing scores 99.83% accuracy and catches zero fraud. So accuracy was rejected, and ROC-AUC with it. Compared five imbalance strategies under leakage-free cross-validation; class weighting won, XGBoost took the best PR-AUC. Includes SHAP + permutation importance and a chronological drift test.
**PR-AUC 0.825 · precision 0.97 · 6 ms per transaction**
`Python` `XGBoost` `scikit-learn` `imbalanced-learn` `SHAP` `joblib`
🔗 **[View repo →](https://github.com/nusukhan/credit-card-fraud-detection)**

---

### 💻 Laptop Price Prediction — *live app*
A neural network that estimates a laptop's price from its specs, trained on 1,275 laptops and deployed with its full preprocessing pipeline so it predicts in a browser in ~200 ms. Most of the work was feature engineering messy text fields into usable columns.
**R² 0.79 · mean error €231 · beats linear baseline (0.76)**
`Python` `TensorFlow/Keras` `scikit-learn` `pandas` `Streamlit`
🔗 **[Live app ↗](https://laptop-price-nusrat.streamlit.app)** · **[View repo →](https://github.com/nusukhan/laptop-price-prediction)**

---

### 🌴 Palm Tree Counter
An object-detection model that counts palm trees in aerial/drone imagery — a box around every tree and a live count on each video frame. Fine-tuned with transfer learning, with an OpenCV frame-by-frame video pipeline.
**mAP50 0.994 · mAP50-95 0.918 · 817 video frames processed**
`Python` `YOLO (Ultralytics)` `OpenCV` `Roboflow` `Google Colab`
🔗 **[View repo →](https://github.com/nusukhan/palm-tree-counter)**

---

### ✍️ Handwritten Digit Recognition
Finds handwritten digits inside an image and labels them — built from raw pixels to prediction, not wrapping a pre-trained model. An SVM trained on 1,797 images, plus a complete OpenCV detection pipeline (grayscale → blur → threshold → contours → predict → draw box).
**98.89% accuracy on 450 unseen images · 10 classes**
`Python` `scikit-learn` `OpenCV` `NumPy` `Matplotlib`
🔗 **[View repo →](https://github.com/nusukhan/digit-recognition-opencv)**

---

### 🍎 Fruit Image Classification (CNN)
A convolutional network that names the fruit in a photo and reports its confidence — built to understand what a CNN does differently from a plain network. Trained on 2,160 images across 4 classes, evaluated on 721 held-out images.
**100% test accuracy on Fruits-360 (clean dataset — honest caveat in the repo)**
`Python` `TensorFlow/Keras` `scikit-learn` `NumPy` `Google Colab`
🔗 **[View repo →](https://github.com/nusukhan/fruit-classification-cnn)**

---

### 🫁 Pneumonia Detection from Chest X-Rays
A CNN (built from scratch) that classifies chest X-rays as Normal or Pneumonia with a confidence score, served through a FastAPI + web interface. Handled a 3:1 class imbalance with class weights, rebuilt a proper validation split, and prioritised recall — because in medical AI a missed positive is the costliest error. *Educational project, not a diagnostic tool.*
**91% test accuracy · pneumonia recall 0.96 · normal recall 0.82 (624 unseen images)**
`Python` `TensorFlow/Keras` `FastAPI` `Pillow` `NumPy` `Google Colab`
🔗 **[View repo →](https://github.com/nusukhan/pneumonia-detection)**

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=nusukhan&show_icons=true&theme=radical" alt="Nusrat's GitHub stats" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=nusukhan&layout=compact&theme=radical" alt="Top languages" />
</p>

---

<p align="center"><i>Building, measuring, and shipping — one project at a time.</i></p>
