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
│
├── data/
│   ├── raw/                          ← 920 original .wav files (local only)
│   ├── audio_and_txt_files/          ← 920 annotation .txt files
│   ├── patient_diagnosis.csv         ← disease labels
│   ├── filename_differences.txt      ← dataset documentation
│   └── filename_format.txt           ← dataset documentation
│
├── output/
│   ├── preprocessed/                 ← 920 cleaned .wav files (local only)
│   ├── features/
│   │   ├── mfcc_features.npy         ← MFCC feature matrix (920 × 26)
│   │   └── file_names.npy            ← filenames list
│   └── models/
│       ├── best_model.keras          ← V1 model (too large, local only)
│       ├── best_model_v2.keras       ← V2 baseline CNN
│       ├── best_model_v3.keras       ← V3 deeper CNN (best single model)
│       ├── best_model_v4.keras       ← V4 CNN with augmentation
│       └── label_classes.npy         ← disease class names
│
├── notebooks/
│   ├── preprocessing.ipynb           ← Stage 1
│   ├── mfcc_extraction.ipynb         ← Stage 2
│   └── cnn_training.ipynb            ← Stage 3
│
├── .gitignore                        ← excludes raw, preprocessed, large model
└── README.md                         ← project description
```
