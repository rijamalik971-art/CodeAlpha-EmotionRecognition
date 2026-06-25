# Emotion Recognition from Speech
### CodeAlpha Machine Learning Internship — Task 2

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square&logo=tensorflow)
![Dataset](https://img.shields.io/badge/Dataset-RAVDESS-purple?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-48.61%25-green?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

## Project Overview
This project recognizes human emotions from speech audio using **Deep Learning** and **Speech Signal Processing**. The model is trained on the **RAVDESS dataset** and can classify 8 different emotions.

## Objective
Recognize the following emotions from speech audio:
😠 Angry | 😌 Calm | 🤢 Disgust | 😨 Fearful | 😊 Happy | 😐 Neutral | 😢 Sad | 😲 Surprised

## Dataset
| Property | Details |
|----------|---------|
| Name | RAVDESS (Ryerson Audio-Visual Database) |
| Total Files | 1440 audio files |
| Actors | 24 (12 Male, 12 Female) |
| Emotions | 8 |
| Format | .wav |

## Feature Extraction
| Feature | Description |
|---------|-------------|
| MFCCs (40) | Mel-Frequency Cepstral Coefficients |
| Chroma (12) | Pitch class features |
| Mel Spectrogram (128) | Frequency-time representation |
| **Total Features** | **180 per audio file** |

##  Model Architecture
Dense(512) + BatchNormalization + Dropout(0.3)
Dense(256) + BatchNormalization + Dropout(0.3)
Dense(128) + BatchNormalization + Dropout(0.3)
Dense(64) + Dropout(0.2)
Dense(8) + Softmax

##  Results
| Metric | Value |
|--------|-------|
| Test Accuracy | 48.61% |
| Best Emotion | Surprised (56%) |
| Total Parameters | 269,256 |

##  Tech Stack
| Tool | Purpose |
|------|---------|
| Python 3.10+ | Programming language |
| TensorFlow/Keras | Deep learning model |
| Librosa | Audio feature extraction |
| NumPy/Pandas | Data manipulation |
| Matplotlib/Seaborn | Visualization |
| Google Colab | Training (Free GPU) |

##  How to Run
1. Open `codeAlpha_task_2.ipynb` in Google Colab
2. Runtime → Change runtime type → **GPU**
3. Run all cells
4. Model will train automatically

## Author
**Rija Malik**
GitHub: [@rijamalik971-art](https://github.com/rijamalik971-art)

## 🏢 Internship
Completed as part of **CodeAlpha Machine Learning Internship**
- 🌐 [www.codealpha.tech](https://www.codealpha.tech)
