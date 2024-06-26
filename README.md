# Multimodal-Medical-Diagnosis-System-For-Alzheimer-s-Disease

We have developed a deep learning-based framework for the early detection of Alzheimer’s disease progression utilizing multimodal data comprising MRI images, demographic features, and cognitive scores, while ensuring model explainability using Grad-CAM to provide insights into the regions of interest within the MRI images that contribute to the classification decisions

The dataset (MRI scans, Demographic and Cognitive Scores) used for training are from the [Alzheimer Disease Neuroimaging Initiative (ADNI)](http://adni.loni.usc.edu/)

### Methodology
![image](https://github.com/durga207/Multimodal-Medical-Diagnosis-System-For-Alzheimer-s-Disease/assets/78926897/d05deee3-6d5b-463b-8d6a-3e60b7eee089)

### Code Structure

- __mri_preprocess :__ Script to automate the preprocessing steps for the MRI scans. This includes - Reorientation, Bias Field Correction, MN152 Registration, Skull Stripping
- __cognitive_and_demographic_preprocessing :__ Preprocessing the cognitive and demographic features. This includes steps like data cleaning and normalization
- __model_gradcam :__ 3DCNN + LSTM model for Alzheimer’s Disease Temporal Progression Prediction. Includes Grad-CAM implementation and visualization for explainability
- __experimentation_modalities :__ Experimentation with different combinations of modalities - MRI only, MRI + Demographic, MRI + Cognitive, MRI + Demographic + Cognitive
- __experimentation_fusion :__ Experimentation with different fusion strategies - early and late fusion
