# Retinal OCT Disease Classification with ViT + Explainability

Fine-tuning a Vision Transformer (ViT) on retinal OCT images for 4-class disease 
classification, with a comparative explainability analysis between Grad-CAM and 
Attention Rollout.

## Overview

Optical Coherence Tomography (OCT) B-scans are classified into four categories:

| Class | Condition | Clinical Significance |
|-------|-----------|----------------------|
| CNV | Choroidal Neovascularization | Abnormal vessel growth; wet AMD |
| DME | Diabetic Macular Edema | Intraretinal fluid; diabetic retinopathy |
| DRUSEN | Drusen deposits | RPE elevations; early dry AMD |
| NORMAL | Healthy retina | Reference class |

This project fine-tunes a Vision Transformer (ViT) on retinal OCT B-scans to classify 
four macular conditions: CNV, DME, DRUSEN, and NORMAL. To investigate model transparency, 
we compare two explainability methods — Grad-CAM and Attention Rollout — and evaluate 
which better localizes clinically relevant anatomy in transformer-based medical image 
classification.

The full tutorial is available in the Jupyter Notebook: `OCT_ViT_Classification.ipynb`

## Dataset

[Kermany2017-OCT](https://huggingface.co/datasets/zacharielegault/Kermany2017-OCT)  
Kermany DS et al. (2018). *Cell*, 172(5):1122–1131.  
109,309 labeled retinal OCT images — CNV, DME, DRUSEN, NORMAL  
License: CC BY 4.0
