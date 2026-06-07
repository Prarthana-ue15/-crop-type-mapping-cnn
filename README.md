# Crop Type Mapping from Satellite Imagery Using CNN

**Project Overview**
This project trains and evaluates CNN-based deep learning models to automatically 
classify satellite image patches into 10 land cover and crop type categories. 
The goal is to demonstrate how convolutional neural networks can be applied to 
real-world remote sensing data for agricultural monitoring and crop type mapping.

**Dataset**
- Name: EuroSAT RGB
- Source: ESA Copernicus Sentinel-2 Satellite
- Total Images: 27,000
- Classes: 10 (AnnualCrop, Forest, HerbaceousVegetation, Highway, Industrial, 
  Pasture, PermanentCrop, Residential, River, SeaLake)
- Image Size: 64 × 64 pixels (RGB)
- Dataset Link: https://www.kaggle.com/datasets/nilesh789/eurosat-rgb

**How to Run**
1. Open the Kaggle Notebook: https://www.kaggle.com/code/prarthanap374/machine-learning
2. Click Copy and Edit
3. Add the EuroSAT dataset via + Add Data → search "EuroSAT RGB"
4. Enable GPU: Settings → Accelerator → GPU T4 x2
5. Run all cells in order using Shift + Enter

**Requirements**
All libraries are pre-installed on Kaggle:
- TensorFlow 2.19
- NumPy, Matplotlib, Seaborn
- Scikit-learn, Keras

**Results Summary**
The custom CNN significantly outperformed the ResNet50 transfer learning model. 
This suggests that for small 64×64 satellite image patches, a purpose-built 
architecture trained from scratch is more effective than adapting a model 
pre-trained on everyday photographs.
