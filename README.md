# Lung-Disease-Detection
Sound based lung disease detection

## Project Overview
This project aims to automatically detect lung diseases by analysing 
respiratory sound recordings using machine learning and deep learning techniques.
Diseases targeted include COPD, Pneumonia, Asthma, Bronchiolitis, and more.

## Dataset
- **Source:** Respiratory Sound Database (ICBHI 2017)
- **Kaggle:** https://www.kaggle.com/datasets/vbookshelf/respiratory-sound-database
- **Total Recordings:** 920 annotated .wav files
- **Patients:** Children, adults, and elderly
- **Diseases Covered:**
  - COPD (Chronic Obstructive Pulmonary Disease)
  - Pneumonia
  - Asthma
  - Bronchiolitis
  - URTI (Upper Respiratory Tract Infection)
  - LRTI (Lower Respiratory Tract Infection)
  - Bronchiectasis
  - Healthy (Normal)

## Raw Audio Files
The raw audio files are too large to upload in GitHub. 
so i will uplaod the updated project folder drive link soon :)

## Project Structure
```
lung_sound_project/
├── data/
│   └── raw/                    ← original 920 .wav files
├── output/
│   ├── preprocessed/           ← cleaned 920 .wav files
│   └── features/               ← NEW
│       ├── mfcc_features.npy   ← feature matrix (920 x 26)
│       └── file_names.npy      ← filenames list
└── notebooks/
    └── preprocessing.ipynb
```
