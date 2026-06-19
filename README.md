# 🎙️ Audio Forensics: Detecting AI-Generated Voices

## Overview

Audio Forensics: Detecting AI-Generated Voices is a machine learning project that identifies whether an audio recording is a Human Voice or an AI-Generated Voice.

The system extracts multiple acoustic features from audio recordings and uses an ensemble machine learning model to classify the voice source with a confidence score.

---

## Features

✔ Human vs AI Voice Detection

✔ Acoustic Feature Extraction

✔ Audio Data Augmentation

✔ Ensemble Machine Learning Model

✔ Confidence Score Prediction

✔ Cross-Validation Evaluation

✔ Model Saving and Loading using Pickle

---

## Technologies Used

- Python
- Librosa
- NumPy
- Scikit-Learn
- Gradient Boosting Classifier
- Support Vector Machine (SVM)
- Pickle

---

## Project Structure

Audio-Forensics-AI-Voice-Detection/

├── dataset/

│   ├── human/

│   └── ai/

├── main.py

├── voice_detector_model.pkl

├── feature_scaler.pkl

├── test.wav

├── README.md

└── requirements.txt

---

## Audio Features Extracted

### MFCC Features
- MFCC
- Delta MFCC
- Delta-Delta MFCC

### Spectral Features
- Spectral Centroid
- Spectral Bandwidth
- Spectral Rolloff
- Spectral Flatness
- Zero Crossing Rate

### Harmonic Features
- Chroma Features
- Tonnetz Features

### Energy Features
- RMS Energy
- Mel Spectrogram Features

---

## Data Augmentation Techniques

To improve model performance, the following augmentations are applied:

- Pitch Shift (+2)
- Pitch Shift (-2)
- Time Stretch (Fast)
- Time Stretch (Slow)
- Gaussian Noise Addition
- Volume Scaling

---

## Machine Learning Model

The project uses an Ensemble Voting Classifier consisting of:

### Gradient Boosting Classifier
- 200 Estimators
- Learning Rate = 0.05

### Support Vector Machine
- RBF Kernel
- Balanced Class Weights
- Probability Estimation Enabled

The final prediction is generated using Soft Voting.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/audio-forensics-ai-voice-detection.git
cd audio-forensics-ai-voice-detection
```

Install required libraries:

```bash
pip install -r requirements.txt
```

---

## Usage

Run the program:

```bash
python main.py
```

Example Output:

```text
Result: AI Generated Voice

Confidence: 96.8%

Human: 3.2%
AI: 96.8%
```

---

## Applications

- Deepfake Voice Detection
- Audio Forensics
- Cybersecurity
- Media Verification
- Fake Audio Identification
- Voice Authentication Systems

---

## Future Improvements

- Deep Learning Models (CNN/LSTM)
- Real-Time Voice Detection
- Web Interface
- Mobile Application
- Multi-Language Support

---
