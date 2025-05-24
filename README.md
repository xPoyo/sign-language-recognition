
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


## 📁 Project Structure

```
sign-language-recognition/
│                   
├── extraccion_de_imagenes.py  # Captures hand landmark data
├── dataset.py                 # The script processes labeled hand gesture images stored in subdirectories under ./data/.
├── randomforest.py            # Trains the recognition model
├── modelo final.py            # Real-time gesture recognition
└── README.md                  # This file
```

## 🧪 Getting Started



### 1. Capture Training Data

Run the script to start capturing gesture data:

```bash
extraccion_de_imagenes.py
```

### 2. Create the dataset

```bash
python dataset.py
```
This step creates the feature dataset used to train the sign recognition model.

### 3. Train the Model

```bash
python randomforest.py
```

This will train a classifier and save the model.

### 4. Run Real-Time Recognition

```bash
python modelo final.py
```

The system will use your webcam to recognize signs in real-time.

## ✅ Expected Results

- Accurate recognition of a predefined set of hand gestures.
- Easy expansion by adding more sign classes.
- A foundation for inclusive communication tools.

## 📌 Notes

- Good lighting and a neutral background will improve recognition accuracy.
- Consistency in hand position during data capture is crucial for model performance.

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
