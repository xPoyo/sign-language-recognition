
# Sign Language Recognition using MediaPipe and OpenCV

This project implements a real-time sign language recognition system using computer vision techniques. It leverages **MediaPipe** and **OpenCV** for video capture and hand landmark detection, and trains a machine learning model to recognize hand gestures representing sign language.

## 🚀 Project Overview

The goal of this project is to improve communication accessibility for the deaf and hard-of-hearing community by interpreting sign language through a webcam. The system performs the following tasks:

- Real-time video capture using OpenCV.
- Hand landmark detection using MediaPipe.
- Preprocessing and storage of hand pose data.
- Training a gesture classification model.
- Real-time gesture recognition and display.

## 🧰 Technologies Used

- [Python](https://www.python.org/)
- [OpenCV](https://opencv.org/)
- [MediaPipe](https://developers.google.com/mediapipe)
- [NumPy](https://numpy.org/)
- [scikit-learn](https://scikit-learn.org/)
- [TensorFlow](https://www.tensorflow.org/) *(optional, for neural network models)*

## 📁 Project Structure

```
sign-language-recognition/
│
├── data/                      # Training data (landmark points)
├── model/                     # Trained models
├── notebooks/                 # Jupyter Notebooks for experiments
├── utils/                     # Utility scripts
├── capture_data.py            # Captures and stores hand landmark data
├── train_model.py             # Trains the recognition model
├── recognize.py               # Real-time gesture recognition
├── requirements.txt           # Project dependencies
└── README.md                  # This file
```

## 🧪 Getting Started

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Capture Training Data

Run the script to start capturing gesture data:

```bash
python capture_data.py
```

You'll be prompted to enter the label of the sign. Then, the system will start recording hand landmarks.

### 3. Train the Model

```bash
python train_model.py
```

This will train a classifier and save the model to the `model/` directory.

### 4. Run Real-Time Recognition

```bash
python recognize.py
```

The system will use your webcam to recognize signs in real-time.

## ✅ Expected Results

- Accurate recognition of a predefined set of hand gestures.
- Easy expansion by adding more sign classes.
- A foundation for inclusive communication tools.

## 📌 Notes

- Good lighting and a neutral background will improve recognition accuracy.
- Consistency in hand position during data capture is crucial for model performance.
- You can expand the dataset by repeating the data collection process with new labels.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 🤝 Contributions

Contributions are welcome! Feel free to open an issue or fork the repository to propose new signs or improvements.
