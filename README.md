# Analysis of ECG Signals for Arrhythmia Classification

Researchers have utilized various datasets for the analysis of ECG signals to classify arrhythmias. Among these datasets, two widely used public databases are the **PhysioNet Challenge 2017 training database** and the **MIT-BIH database**, which is accessible on PhysioNet.

---

## MIT-BIH Database

For binary classification, the following datasets from the MIT-BIH database have been employed:  
1. **MIT-BIH Atrial Fibrillation Database (AF)**  
2. **MIT-BIH Normal Sinus Rhythm Database (NSR)**  

### Key Details:  
- **Sampling Rate**:  
  - AF dataset: 250 Hz  
  - NSR dataset: 128 Hz  
- **Leads Used**: Both datasets use two leads (ECG1 and ECG2) with a 12-bit Analog to Digital Converter (ADC) resolution. For this study, only the signal from lead one has been used.  
- **Resampling**: The AF dataset, originally sampled at 250 Hz, is resampled to 128 Hz to match the NSR dataset's sampling rate for training purposes.

---

## PhysioNet Challenge 2017 Training Database

For multiclass classification, the **PhysioNet Challenge 2017 training database** is utilized. It contains ECG segments categorized into three different classes: normal, atrial fibrillation (AF), and other abnormalities.

### Key Details:  
- **Total ECG Segments**: 8528 single-lead ECG segments with four target labels, including:  
  - 738 recordings for **atrial fibrillation (AF)**  
  - 5050 recordings for **normal sinus rhythm (NSR)**  
  - 2456 recordings for **other abnormal rhythms**  
  - 284 recordings that were deemed too noisy for use  
- **Sampling Rate**: Original signals are sampled at 300 Hz with a 16-bit ADC resolution.  
- **Downsampling**: The signals are down-sampled to 150 Hz to reduce the computational load of the network.

---

This document provides a concise overview of the datasets and preprocessing steps used in the analysis of ECG signals for arrhythmia classification. 
