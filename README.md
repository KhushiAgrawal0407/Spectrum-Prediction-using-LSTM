# 📌 Overview

- This project explores spectrum occupancy prediction in Cognitive Radio Networks (CRNs) using Long Short-Term Memory (LSTM) models, integrated with Reconfigurable Intelligent Surfaces (RIS) for improved efficiency in Device-to-Device (D2D) communication.

- The goal is to predict whether a spectrum channel will be idle (0) or busy (1) in upcoming time slots, enabling secondary users (SUs) to access the spectrum opportunistically without interfering with primary users (PUs).


# 🚀 Key Features

- Developed an LSTM-based model for spectrum occupancy prediction.

- Implemented synthetic spectrum data generation using a sliding window approach.

- Evaluated using metrics like Accuracy, MSE, Precision, Recall, F1-score, AUC, ROC curves.

- Compared LSTM performance with Random History Model (RHM) and Hidden Markov Model (HMM).

- Achieved 87% accuracy with minimal overfitting.

- System integrates:

  - RIS phase reconfiguration for improved SINR.

  - Energy Harvesting (EH) model with Harvest-Then-Transmit strategy.


# 🛠️ Tech Stack

### - Language/Frameworks:
Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Scikit-learn

### - Model:
LSTM Neural Network

### - Simulation:
Synthetic spectrum occupancy data with temporal correlation


# 📊 Methodology

### - Data Generation & Preprocessing:

  - Binary spectrum occupancy sequences generated synthetically.

  - Input reshaped into sequences of 25 timesteps.

### - Model Architecture:

  - 2 LSTM layers with dropout & batch normalisation.

  - Dense layers for binary classification.

### - Training & Evaluation:

  - 50 epochs, batch size = 32, Adam optimizer.

  - Metrics: Accuracy, MSE, Precision, Recall, F1-score.


# 📈 Results

### - Accuracy:
87.07%

### - MSE:
0.129 (Validation MSE ~0.0985)

### - Precision/Recall/F1:
~0.65

### - ROC AUC (LSTM):
0.83 vs HMM (0.45) & RHM (0.50)


# 📸 Screenshots

## 1. Actual vs Predicted Occupancy

<img width="1397" height="861" alt="Actual vs Predicted Spectrum Occupancy" src="https://github.com/user-attachments/assets/98c52a6e-53c1-480e-99f0-09d1faf11ace" />

## 2. Accuracy/Loss Graph

<img width="1766" height="738" alt="Accuracy and Loss over Epochs" src="https://github.com/user-attachments/assets/d7959bbd-fcc1-4480-bdc2-7be68d6a4e84" />

## 3. Training vs Validation MSE

<img width="1355" height="919" alt="Training vs Validation MSE" src="https://github.com/user-attachments/assets/896dfbc1-83ca-46eb-9d00-c3d4e8915b3b" />

## 4. ROC Curve Comparision between various models

<img width="1065" height="759" alt="ROC Curve Comparision" src="https://github.com/user-attachments/assets/dffa5cae-d0b2-4097-abcd-34466bc31a2a" />

## 5. ROC Curve of LSTM

<img width="1024" height="801" alt="ROC Curve LSTM" src="https://github.com/user-attachments/assets/adb8e610-31b6-4bb9-bdc5-0178fe9a482f" />

## 6. Confusion Matrix

<img width="847" height="787" alt="Confusion Matrix" src="https://github.com/user-attachments/assets/fba5d5ef-a936-4013-8412-aceca2768725" />


# 🔮 Future Work

- Extend with real-world spectrum datasets.

- Explore Transformer and BiLSTM models.

- Integrate RIS optimisation and beamforming.

- Implement energy efficiency and throughput gain analysis.

- Prototype with hardware for real RF spectrum data.


# 👥 Contributors

- Khushi Agrawal

- Kunjika Gupta

- Rishika Parashar

- Supervisor: Dr. Anirudh Agarwal
