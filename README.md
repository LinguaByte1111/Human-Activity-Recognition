# 🧍 Human Activity Recognition (HAR) using Live Video and Deep Learning

This project implements a **real-time Human Activity Recognition system** using a pre-trained deep learning model built with TensorFlow/Keras. The system captures live video from a webcam and classifies human actions such as walking, sitting, standing, and more.

---

## 📚 Table of Contents

- [🧠 Project Overview](#-project-overview)
- [📁 Project Structure](#-project-structure)
- [🔍 Model Details](#-model-details)
- [🚀 How It Works](#-how-it-works)
- [📦 Requirements](#-requirements)
- [▶️ How to Run](#️-how-to-run)
- [🧪 Sample Output](#-sample-output)
- [📌 Notes](#-notes)
- [🧰 Utility Function: Max Subsequence](#-utility-function-max-subsequence)
- [📷 Screenshots (Optional)](#-screenshots-optional)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🧠 Project Overview

The goal of this project is to recognize and classify human activities using a **Convolutional Neural Network (CNN)** trained on image data. The model is capable of identifying various physical states from webcam video in real time.

### Activities Detected

- 🧍 Standing  
- 🪑 Sitting  
- 🛏️ Sleeping  
- 🚶 Walking  
- 🧗 Walking on Stairs  
- ⏹ Control (Default/Idle state)

---

---

## 🔍 Model Details

- **Framework:** TensorFlow / Keras  
- **Input Size:** 150x150 RGB images  
- **Normalization:** Pixel values scaled to `[-1, 1]`  
- **Output:** Softmax classification across **6 activity classes**

---

## 🚀 How It Works

1. Captures live video feed using **OpenCV**.
2. Each frame is:
   - Converted to a **PIL image**
   - Resized to **150x150 pixels**
   - Normalized and reshaped to match the model's input format
3. Model predicts the activity from the processed frame.
4. Predicted label is printed to the console with a timestamp.

---

## 📦 Requirements

Install the dependencies using pip:

```bash
pip install numpy opencv-python tensorflow pillow
```


## ▶️ How to Run

Ensure your webcam is connected and functional.

Run the main script:

Copy
Edit

```bash
python main.py
```
Press q to exit the live video feed.

