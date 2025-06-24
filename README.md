### 🧍 Human Activity Recognition (HAR) using Live Video and Deep Learning
This project implements a real-time Human Activity Recognition system using a pre-trained deep learning model built with TensorFlow/Keras. The system uses your webcam to capture live video and classify human actions such as walking, sitting, standing, and more.

🧠 Project Overview
The goal of this project is to recognize and classify human activities using a Convolutional Neural Network (CNN) trained on image data. The model is capable of identifying various physical states from webcam video in real time.

Activities Detected:
🧍 Standing

🪑 Sitting

🛏️ Sleeping

🚶 Walking

🧗 Walking on Stairs

⏹ Control (Default/Idle state)

📁 Project Structure
bash
Copy
Edit
├── activity4.h5                 # Trained Keras model
├── main.py                      # Live webcam activity classifier
├── utils/
│   └── max_subseq.py            # Utility for max subsequence selection (if required)
🔍 Model Details
Framework: TensorFlow / Keras

Input Size: 150x150 RGB images

Normalization: Image pixel values scaled to [-1, 1]

Output: Softmax classification across 6 classes

🚀 How It Works
Live video is captured using OpenCV.

Each frame is:

Converted to a PIL image

Resized to 150x150 pixels

Normalized and reshaped to match the model input

The model predicts the activity using the trained CNN.

The predicted class is printed in the console along with a timestamp.

📦 Requirements
Install the required Python libraries:

bash
Copy
Edit
pip install numpy opencv-python tensorflow pillow
▶️ How to Run
Make sure your webcam is connected, and run:

bash
Copy
Edit
python main.py
Press q to quit the live feed.

📌 Notes
The model activity4.h5 should be placed in the root directory.

Ensure you have a functional webcam.

Works best in good lighting and when the subject is clearly visible.

🧰 Utility Function: Max Subsequence
A separate utility (max_subseq.py) contains a function to compute the lexicographically largest subsequence of a given string with constraints, potentially used during data preprocessing or filtering steps.

📷 Screenshots (Optional)
Add screenshots of live classification here if available.

🤝 Contributing
Feel free to open issues or submit PRs to improve the model or add new features!

📄 License
MIT License
