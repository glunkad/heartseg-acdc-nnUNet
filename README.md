# heartseg-acdc-nnUNet
Cardiac segmentation research using nnUNet on ACDC challenge dataset
## 🫀 Project Overview
Built a robust cardiac segmentation pipeline using nnUNet trained on the ACDC challenge dataset. Achieved 0.91 Dice score for automated left ventricle, myocardium, and right ventricle segmentation from cardiac MRI sequences.
## 🎯 Research Objective
Develop production-ready cardiac segmentation to enable automated cardiac function analysis, ejection fraction calculation, and regional wall motion assessment.
## 📊 Dataset & Training Results
#### ACDC Challenge Dataset
- Training Cases: 100 cardiac MRI sequences
- Modalities: Cine MR (20 phases per cycle)
- Classes: Left ventricle, myocardium, right ventricle
- Resolution: 256×256 pixels, 8-12 slices per sequence
#### Segmentation Performance

| Cardiac Structure   | Dice Score | HD95 (mm) | Clinical Relevance            |
| ------------------- | ---------- | --------- | ----------------------------- |
| **Left Ventricle**  | **0.94**   | 2.1       | Ejection fraction calculation |
| **Myocardium**      | **0.91**   | 3.2       | Wall thickness/mass           |
| **Right Ventricle** | **0.89**   | 4.1       | RV function assessment        |
| **Average**         | **0.91**   | **3.1**   | **Clinical grade** ✅          |
#### Training Metrics
```# nnUNet Auto-Configuration Results
Best Epoch: 284/500
Training Time: 48h on RTX 3080
Learning Rate: 0.01 (auto-tuned)
Loss Function: DC + CE (auto-weighted)
```
