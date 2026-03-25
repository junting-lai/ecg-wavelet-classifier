# ECG Signal Classification Using Wavelet Transform (LabVIEW)

This project implements an ECG signal classification system using a Daubechies-4 wavelet transform and statistical feature extraction in LabVIEW.

The system loads ECG signals, extracts wavelet-domain features, and classifies heart conditions using threshold-based logic.

---

## Project Overview

This system processes ECG signals through the following pipeline:

ECG Signal Input  
→ Segment Selection  
→ Daubechies-4 Wavelet Transform  
→ Feature Extraction  
→ Threshold Classification  
→ Condition Output

The classifier distinguishes between:

- Normal rhythm
- Atrial tachycardia
- Hyperkalemia
- Hypocalcemia

---

## Signal Processing Pipeline

### Step 1: ECG Signal Input

The program loads ECG waveform data from a user-specified file path and converts it into a time-domain array.

---

### Step 2: Fixed-Length Segment Selection

A fixed-length segment is extracted from the ECG signal to ensure consistent processing across datasets.

---

### Step 3: Wavelet Transform

A Daubechies-4 wavelet transform decomposes the ECG signal into frequency-localized coefficient components.

Wavelet decomposition enables time-frequency analysis of non-stationary biomedical signals such as ECG.

---

### Step 4: Feature Extraction

Statistical features are computed from the wavelet coefficient matrix:

- Maximum value
- Minimum value
- Range (max − min)
- Standard deviation

These features reduce dimensionality while preserving signal characteristics.

---

### Step 5: Classification Logic

Extracted feature values are compared with predefined thresholds to identify signal patterns corresponding to specific cardiac conditions.

Boolean indicators determine whether the signal matches:

- Normal rhythm
- Atrial tachycardia
- Hyperkalemia
- Hypocalcemia

---

## Technologies Used

- LabVIEW
- Wavelet Transform (Daubechies-4)
- Biomedical Signal Processing
- Feature Extraction
- Threshold-based Classification

---

## Applications

This project demonstrates a simplified ECG classification pipeline similar to those used in:

- biomedical signal monitoring systems
- wearable health devices
- diagnostic support systems
- embedded medical instrumentation
