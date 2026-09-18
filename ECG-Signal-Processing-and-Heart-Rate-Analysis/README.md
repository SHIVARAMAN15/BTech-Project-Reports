# ❤️ ECG Signal Processing and Heart Rate Analysis

A Python-based digital signal processing project for preprocessing, analyzing, and interpreting ECG (Electrocardiogram) signals. The project focuses on signal acquisition, noise reduction, Butterworth filtering, frequency-domain analysis using FFT, R-peak detection, and heart-rate estimation.

---

## 📌 Project Overview

The **ECG Signal Processing and Heart Rate Analysis** project explores the application of digital signal processing techniques to biomedical ECG waveform data.

The workflow processes ECG signals from the **MIT-BIH Arrhythmia Database** and performs preprocessing, filtering, frequency-domain analysis, feature extraction, and R-peak detection to estimate heart rate.

The project demonstrates practical implementation of:

- Digital signal processing
- Biomedical signal processing
- Signal filtering
- Noise reduction
- FFT-based frequency analysis
- Feature extraction
- R-peak detection
- Heart-rate estimation
- ECG waveform visualization

---

## 🎯 Objectives

- Acquire and analyze ECG waveform data.
- Preprocess ECG signals to improve signal quality.
- Remove baseline drift and unwanted noise.
- Apply Butterworth bandpass filtering.
- Analyze ECG signals in the frequency domain using FFT.
- Detect R-peaks from processed ECG signals.
- Estimate heart rate from detected R-peaks.
- Visualize raw and processed ECG signals.
- Explore biomedical signal-processing techniques using Python.

---

## 🚀 Key Features

### 📈 ECG Waveform Visualization

Visualizes the acquired ECG waveform in the time domain for signal inspection and analysis.

### 🧹 Signal Preprocessing

Processes raw ECG signals to reduce unwanted components such as:

- Baseline wander
- High-frequency noise
- Motion-related artifacts

### 🔊 Butterworth Bandpass Filtering

A Butterworth bandpass filter is applied to improve ECG signal quality while retaining relevant waveform components.

### 📊 FFT Analysis

Fast Fourier Transform (FFT) is used to analyze the frequency-domain characteristics of the ECG signal.

### ❤️ R-Peak Detection

R-peaks are detected from the processed ECG waveform using ECG processing functionality provided by NeuroKit2.

### 💓 Heart-Rate Estimation

Detected R-peaks are used to estimate heart rate from the ECG waveform.

### 🔬 Feature Extraction

Relevant waveform and physiological features are extracted from the processed ECG signal.

---

## 🧠 Signal Processing Workflow

```text
        ┌─────────────────────────┐
        │     ECG Dataset         │
        │   MIT-BIH Arrhythmia    │
        │       Database          │
        └────────────┬────────────┘
                     │
                     ▼
        ┌─────────────────────────┐
        │     ECG Acquisition     │
        │        Using WFDB       │
        └────────────┬────────────┘
                     │
                     ▼
        ┌─────────────────────────┐
        │   Signal Preprocessing  │
        │                         │
        │ Noise Reduction         │
        │ Baseline-Wander Removal │
        └────────────┬────────────┘
                     │
                     ▼
        ┌─────────────────────────┐
        │ Butterworth Bandpass    │
        │       Filtering         │
        └────────────┬────────────┘
                     │
             ┌───────┴────────┐
             │                │
             ▼                ▼
   ┌─────────────────┐  ┌─────────────────┐
   │  Time-Domain    │  │ Frequency-Domain│
   │    Analysis     │  │   FFT Analysis  │
   └────────┬────────┘  └────────┬────────┘
            │                    │
            └──────────┬─────────┘
                       ▼
             ┌────────────────────┐
             │   R-Peak Detection │
             └──────────┬─────────┘
                        │
                        ▼
             ┌────────────────────┐
             │ Heart-Rate          │
             │ Estimation           │
             └──────────┬─────────┘
                        │
                        ▼
             ┌────────────────────┐
             │ Feature Extraction │
             │ & Visualization    │
             └────────────────────┘
