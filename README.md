# Stevia Adulteration Detection using Hyperspectral Imaging and Machine Learning

## Overview

This repository presents a non-destructive framework for detecting and classifying adulteration in stevia extract using hyperspectral imaging (HSI) and machine learning techniques. Stevia is a widely used natural sweetener with high market value, making it susceptible to adulteration with low-cost substances such as maltodextrin and sodium saccharin. Traditional chemical-based detection methods are often destructive, time-consuming, and laboratory-dependent.

The proposed system leverages both spatial and spectral information from hyperspectral images to provide a fast, scalable, and accurate alternative for stevia quality assessment.

---

## Key Contributions

- First known application of hyperspectral imaging in stevia adulteration detection
- Detection sensitivity down to 5% adulteration concentration
- Pixel-level spatial–spectral analysis enabling detection of non-uniform adulterant distribution
- Comprehensive comparison of feature extraction and feature selection techniques
- Evaluation of multiple machine learning classifiers for robust detection
- Achieved classification accuracy up to 98.6%

---

## Experimental Setup

- Imaging Device: Specim IQ hyperspectral camera  
- Image Dimensions: 512 × 512 × 204  
- Spectral Range: 400–1000 nm  
- Illumination: Dual halogen lamps under controlled dark-room conditions  

### Samples
- Pure stevia extract  
- Stevia adulterated with maltodextrin (5%, 15%)  
- Stevia adulterated with sodium saccharin (5%, 15%)  

All samples were ground to a uniform particle size and placed in transparent petri dishes for hyperspectral image acquisition.

---

## Methodology

### 1. Preprocessing

- Reflectance calibration and normalization
- Region of Interest (ROI) extraction
- Savitzky–Golay filtering for spectral noise reduction
- Min–Max scaling for intensity normalization
- Spatial data augmentation using image rotations

---

### 2. Feature Extraction

The following spatial and spectral feature extraction techniques were implemented:

- Linear Discriminant Analysis (LDA)
- Factor Analysis
- 1D Wavelet Transform
- Morphological Profiles
- 2D Wavelet Transform

---

### 3. Feature Selection

To retain the most discriminative features and reduce dimensionality, the following feature selection methods were evaluated:

- Information Gain
- Fisher Score
- Chi-Square Test
- Relief Algorithm
- Maximum Relevance Minimum Redundancy (mRMR)

---

### 4. Classification Models

The extracted and selected features were classified using:

- Support Vector Machine (SVM)
- Random Forest (RF)
- Multinomial Logistic Regression (MLR)

- Training/Test Split: 80% / 20%  
- Validation: Cross-validation with multiple experimental trials

---

## Results

- Fisher Score combined with Random Forest achieved the highest accuracy of 98.6%
- LDA-based feature extraction consistently produced strong classification performance
- Feature extraction methods generally outperformed feature selection techniques
- Reliable detection was achieved even at low adulteration levels (5%)

---

## Advantages Over Conventional Methods

| Conventional Methods | Proposed System |
|----------------------|-----------------|
| Destructive analysis | Non-destructive analysis |
| Laboratory dependent | Portable and scalable |
| Limited sampling | Full spatial coverage |
| Time-intensive | Fast and automated |

---


## Applications

- Food quality assurance and safety
- Industrial stevia processing
- Regulatory inspection and compliance
- Non-destructive analysis of powdered food products
