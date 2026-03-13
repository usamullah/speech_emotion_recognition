# Speech Emotion Recognition (SER) using CNN

This project implements a Speech Emotion Recognition (SER) system using Deep Learning. It leverages a 1D Convolutional Neural Network (CNN) to classify human emotions from audio recordings. The model is trained on a combination of four widely used datasets: TESS, RAVDESS, SAVEE, and CREMA-D.

## 🚀 Project Overview

The goal of this project is to accurately identify emotions in human speech. Speech emotion recognition has numerous applications in customer service, healthcare, and human-computer interaction.

### Key Features:
- **Comprehensive Data Processing**: Integrates four major audio datasets.
- **Advanced Feature Extraction**: Uses `librosa` to extract MFCCs, Chroma, and Mel Spectrogram features.
- **Deep Learning Model**: Implements a robust 1D CNN architecture for high-accuracy classification.
- **Visualizations**: Includes waveplots, spectrograms, and performance metrics (confusion matrix, loss/accuracy curves).

---

## 📊 Datasets Used

The project combines audio files from several sources to build a diverse and robust training set:
1. **RAVDESS**: The Ryerson Audio-Visual Database of Emotional Speech and Song.
2. **CREMA-D**: Crowd-sourced Emotional Multimodal Actors Dataset.
3. **TESS**: Toronto Emotional Speech Set.
4. **SAVEE**: Surrey Audio-Visual Emotional Database.

The combined dataset includes emotions like **Neutral, Calm, Happy, Sad, Angry, Fearful, Disgust, and Surprised**, categorized by both male and female speakers.

---

## 🛠️ Model Architecture

The core of the system is a **1D Convolutional Neural Network** built with Keras/TensorFlow. The architecture includes:
- **Input Layer**: Processes the extracted audio features.
- **Multiple Conv1D Layers**: For spatial feature learning in the audio signal.
- **Batch Normalization**: To speed up training and provide stability.
- **Max Pooling Layers**: For down-sampling and feature reduction.
- **Flatten & Dense Layers**: To condense learned features into the final classification.
- **Output Layer**: A Softmax layer with 14 units representing the gendered emotion classes.

---

## 📈 Performance

The model achieved an impressive **93.54% Accuracy** on the testing dataset.

| Metric | Result |
| :--- | :--- |
| **Model Accuracy** | 93.54% |
| **Optimization** | RMSprop |
| **Loss Function** | Categorical Crossentropy |

---

## 📂 Installation and Usage

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Libraries: `tensorflow`, `keras`, `librosa`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

### Setup
1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open `speech_emotion_recognition.ipynb` in your Jupyter environment.
4. Ensure your audio datasets are correctly pathed in the notebook.
5. Run cells sequentially to process data, train the model, and evaluate results.

---

## 📊 Visualizations

The project provides detailed insights into the audio data:
- **Waveplots**: Visual representation of the sound signal over time.
- **Spectrograms**: Frequency-domain representation showing how the signal's frequency content changes over time.
- **Confusion Matrix**: To analyze the model's precision and recall across different emotion categories.

---

## 📧 Contact
For any questions or feedback, feel free to reach out.
usamullah093@gmail.com
