# machine_learning_project

This repository contains the implementation of a deep learning pipeline for ECG Arrhythmia Classification using the MIT-BIH Arrhythmia Database. The project compares the performance of a baseline 1D Convolutional Neural Network (CNN) against various Long Short-Term Memory (LSTM) architectures for classifying six distinct heartbeat types (Normal, LBBB, RBBB, Atrial Premature, Supraventricular Premature, and Ventricular Premature). The pipeline includes comprehensive signal preprocessing (bandpass filtering, normalization, and truncation) and utilizes a rigorous evaluation framework with 5-fold cross-validation on patient-specific training/testing splits. Performance is benchmarked using accuracy, F1-score, and 
F
β
​
  metrics to account for class imbalance. The project is fully implemented in Python using TensorFlow/Keras and is designed for reproducibility and experimentation with sequential ECG data.

* Task: Multi-class classification of ECG heartbeats (N, L, R, A, S, V).

* Data: MIT-BIH Arrhythmia Database (PhysioNet), preprocessed with 0.001-15Hz Bandpass Filtering and Z-score Normalization.

* Models: Custom 1D-CNN Baseline vs. Configurable LSTM Architectures (varying layers, units, and dropout).

* Validation: Patient-independent split (Record IDs 1xx for Train/CV, 2xx for Test) with 5-Fold Cross-Validation.

* Tech Stack: Python 3, TensorFlow/Keras, WFDB, Scikit-learn, Matplotlib.

