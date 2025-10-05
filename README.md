# Affect-Net
This repository contains a complete structure and starter code for the assignment: facial expression (categorical) and valence/arousal (continuous) prediction using CNN baselines. It includes modular code, training/evaluation scripts, metrics.

# CNN Architectures for Facial Expression and Affect Recognition

## 1. Network Details
Models: ResNet50, VGG16, Custom CNN
Input: 224x224x3
Optimizer: Adam, LR=0.001, Batch size=32, Epochs=20

## 2. Dataset Splits
Total samples: 3999
Train: 3199 (80%)
Validation: 800 (20%)

## 3. Performance Measures (summary)
### ResNet50
Accuracy: 0.1500; F1:0.0783; AUC:0.5190
Valence RMSE:0.4699, CORR:0.0096
Arousal RMSE:0.3848, CORR:0.1068

### VGG16
Accuracy:0.3175; F1:0.3110; AUC:0.6100
Valence RMSE:0.4325, CORR:0.4200
Arousal RMSE:0.3667, CORR:0.3237

### Custom CNN
Accuracy:0.1963; F1:0.1679; AUC:0.5407
Valence RMSE:0.4637, CORR:0.1716
Arousal RMSE:0.3832, CORR:0.1717

Observations: VGG16 outperformed others across most metrics. ResNet50 underperformed — likely due to overfitting on limited data. Custom CNN is fast but less accurate.


