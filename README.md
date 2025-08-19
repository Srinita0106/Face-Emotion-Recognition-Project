# Face-Emotion-Recognition-Project


This project focuses on deep learning-based **Facial Emotion Recognition**. It enables real-time identification of emotions from human faces using images or webcam video, making it a strong demonstration of AI and computer vision skills. The system is built end-to-end: from data preprocessing and model training to live inference.



### Key Features

- **Emotion Classes Recognized:** Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral
- **Model:** Custom Convolutional Neural Network (CNN) using Keras and TensorFlow
- **Real-Time Prediction:** Live webcam emotion detection with OpenCV
- **Data Augmentation:** ImageDataGenerator for robust training (rotation, shear, zoom, flip)
- **Visualization:** Overlays emotion on detected faces in video stream
- **Extensible:** Adaptable to new datasets or more/other classes



### Tech Stack

| Component              | Technology/Tool                           |
|------------------------|-------------------------------------------|
| Programming Language   | Python 3.11                               |
| Deep Learning          | Keras (TensorFlow backend)                |
| Data Manipulation      | NumPy                                     |
| Visualization         | Matplotlib, OpenCV                         |
| Face Detection        | OpenCV Haar Cascade Classifier             |
| Model Format           | HDF5 (`.h5`), Keras Native                |



### Workflow

1. **Data Preparation:** Dataset of facial images (grayscale, 48x48 pixels) sorted into 7 emotion class folders for training and testing (~28,709 train, ~7,178 test).
2. **Preprocessing:** Images normalized and augmented for better generalization and robustness.
3. **Model Building:** CNN with multiple convolution, pooling, and dropout layers, ending with softmax classification over 7 emotions.
4. **Training:** Model trained for 50+ epochs, accuracy stabilized around 60% on test data.
5. **Saving:** Trained model saved in HDF5 format for reuse.
6. **Live Inference:** Uses OpenCV to capture face from webcam and predict emotion, showing class on screen.
7. **Extensible Notebook:** Easily modifiable for further experiments or additional emotion categories.



