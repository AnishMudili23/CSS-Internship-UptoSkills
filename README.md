# CSS-Internship-UptoSkills

# 🚨 Real-Time CCTV Chain Snatching Detection Using Deep Learning

## 📌 Project Overview

This project focuses on detecting **chain snatching incidents from CCTV surveillance videos** using deep learning.

The system automatically analyzes surveillance footage and classifies videos into:

🟢 **Normal Activity**
🔴 **Chain Snatching Incident**

The goal is to assist surveillance systems by **automatically detecting suspicious activities**, improving public safety and reducing the need for constant manual monitoring.

---

# 🎯 Problem Statement

Manual monitoring of CCTV footage is:

* Time consuming
* Prone to human fatigue
* Difficult when dealing with large volumes of video data

This project aims to:

* Automatically analyze CCTV footage
* Detect chain snatching activities
* Reduce false alarms
* Improve surveillance efficiency

---

# 📂 Datasets Used

## 1️⃣ Chain Snatching & Anomaly Detection Dataset (Primary Dataset)

Dataset Link
[https://www.kaggle.com/datasets/siddhantborude777/chain-snatching-and-anomaly-detection-dataset](https://www.kaggle.com/datasets/siddhantborude777/chain-snatching-and-anomaly-detection-dataset)

Folders used:

* `chain_snatching_videos`
* `normal_videos`

Description:

Contains real chain snatching incidents and normal activity videos used to train the binary classification model.

---

## 2️⃣ Action Recognition Test Videos – Phase 3

Dataset Link
[https://www.kaggle.com/datasets/yashtisahu/action-videos](https://www.kaggle.com/datasets/yashtisahu/action-videos)

Videos used from this dataset:

* `normal_walking`
* `shaking_hands`
* `snatching`

Folder excluded:

❌ `punching`

Reason for exclusion:

* Introduced visual confusion
* Reduced model validation accuracy
* Added noise to the dataset

---

## 3️⃣ Dataset Not Used

Dataset:
[https://www.kaggle.com/datasets/rajasree25/actionvideos-upd](https://www.kaggle.com/datasets/rajasree25/actionvideos-upd)

Reason for exclusion:

* Introduced significant dataset noise
* Reduced training accuracy
* Created unstable validation results

---

# 🧠 Model Architecture

Model: **3D ResNet-18**

Framework: **PyTorch**

GPU Used: **Kaggle GPU (P100)**

Binary Classification:

```
0 → Normal Activity
1 → Chain Snatching
```

The model processes video frames and learns **spatio-temporal features** to detect abnormal events.

---

# ⚙️ Workflow

The complete pipeline includes:

1️⃣ Data Collection
2️⃣ Dataset Cleaning & Filtering
3️⃣ Frame Extraction from Videos
4️⃣ Dataset Balancing
5️⃣ Model Training
6️⃣ Model Validation
7️⃣ Video Prediction
8️⃣ Excel Output Generation

---

# 📊 Evaluation Metrics

The model performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

# ✅ Final Accuracy

Final Accuracy Achieved:

**~98.33%**

Performance summary:

* Correct predictions: **~295 / 300 videos**
* Misclassifications: **5 videos**
* Very low false positives
* Strong detection capability

---

# 📈 Results

The trained model successfully distinguishes between:

✔ Normal activities
✔ Chain snatching incidents

The system demonstrates reliable detection performance on CCTV video data.

---

# 📁 Output

The system generates an **Excel report** containing:

* Video Name
* True Label
* Predicted Label
* Confidence Score
* Correct / Incorrect prediction

Example output file:

```
video_predictions.xlsx
```

---

# 🔥 Key Features

* High detection accuracy (~98%)
* Reduced dataset noise through filtering
* GPU-accelerated training
* Clean binary classification
* Designed for CCTV surveillance applications

---

# 🚀 Future Improvements

Possible future improvements include:

* Real-time CCTV deployment
* Alert system integration (SMS / notifications)
* Transformer-based video models
* Larger and more diverse datasets
* Edge device deployment

---

# ⚙️ Installation

Install required libraries:

```
pip install -r requirements.txt
```

---

# ▶️ How to Run

1. Download datasets from Kaggle
2. Place datasets in the dataset folder
3. Run the notebook

```
cnnfinalold-new.ipynb
```

The notebook will:

* train the model
* test on videos
* generate prediction results

---

# 👩‍💻 Authors

* **Anish**
* **Rajasree**
* **Nandana U**

---

# 📌 Conclusion

This project demonstrates how **deep learning can assist surveillance systems** by automatically detecting criminal activities such as chain snatching.

By carefully selecting and filtering datasets, the model achieves **high accuracy and reliable performance**, making it a promising solution for **AI-based CCTV monitoring systems**.

---
