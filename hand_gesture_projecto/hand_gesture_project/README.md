# Hand Gesture Recognition with Optical Flow & MediaPipe

This project is focused on **real-time hand gesture recognition** using **MediaPipe**, **Optical Flow (Lucas-Kanade & Farneback)**, and machine learning models like **KNN** or **SVM** for classification.

---

## 📌 Features

- 🔎 Real-time **hand tracking** using MediaPipe
- 🌊 Optical Flow computation (Lucas-Kanade & Farneback)
- 📊 Histogram-based **feature extraction**
- 🧠 Train gesture classifiers (KNN/SVM)
- 🕹️ Real-time gesture **prediction**
- 💾 Record custom gestures with labels and save them to CSV

---

## 🗂️ Project Structure

```bash
hand_gesture_project/
│
├── record_gestures.py           # Record labeled gestures and save feature histograms
├── train_model.py               # Train an SVM or KNN model using the recorded gestures
├── predict_gestures.py          # Real-time gesture prediction using the trained model
│
├── utils/
│   ├── optical_flow.py          # Lucas-Kanade & Farneback flow computation
│   ├── feature_extraction.py    # Flow histogram + trajectory feature extraction
│   └── visualization.py         # Draw flow vectors and dense flow visualization
│
├── models/
│   └── gesture_recognizer.pkl   # Trained ML model (output)
│
└── data/
    └── gesture_data.csv         # Stored histogram features with labels
