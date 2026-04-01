# COMP6001 Assignment 1 – Image Restoration and Object Detection

## Student Information
**Name:** Ibrahim Iftekhar Khan  
**Student ID:** A1986169  

---

## Project Overview
This project investigates the effect of motion blur on object detection performance and evaluates whether image restoration (deblurring) improves detection results. The project includes image restoration, object detection experiments, dataset preparation, model fine-tuning, and performance evaluation.

---

## Dataset
The GoPro Deblur Dataset was used in this project. The dataset contains paired blurred and sharp images captured under real motion blur conditions. Due to computational limitations, a subset of 100 matched blurred–sharp image pairs was used for the experiments.

---

## Methods

### 1. Image Deblurring
**Method used:** Richardson–Lucy Deconvolution  
**Evaluation metrics:**
- PSNR (Peak Signal-to-Noise Ratio)
- SSIM (Structural Similarity Index)

**Average Results:**
- PSNR = 24.83  
- SSIM = 0.7467  

---

### 2. Object Detection
**Model used:** YOLOv8 (Pretrained)

Detection was performed on:
- Blurred images
- Deblurred images
- Sharp images

Detection counts and confidence scores were compared to evaluate the impact of image restoration on object detection performance.

---

### 3. Fine-Tuning
Since the dataset did not include object detection labels, pseudo-labels were generated using YOLOv8 on sharp images. The model was first fine-tuned using YOLOv8n and then improved using a YOLOv8s model with data augmentation and additional training epochs.

**Final Improved Model Results:**
- Precision = 0.6817
- Recall = 0.6383
- mAP@50 = 0.7070
- mAP@50-95 = 0.5631

The improved model produced higher detection counts on deblurred images compared to blurred images, showing that restoration combined with model fine-tuning improves detection performance.

---

## Repository Structure
comp6001_assignment1/
│
├── notebooks/ # Jupyter and Colab notebooks
├── outputs/ # Plots, metrics, and generated results
├── data/ # Dataset (not included in repo due to size)
├── report/ # Final report
├── slides/ # Presentation slides
├── ai_logs/ # AI usage documentation
├── README.md
├── requirements.txt
└── .gitignore


---

## How to Run the Project

### Local (Deblurring and Evaluation)
1. Install Python 3.10+
2. Install required libraries:
pip install -r requirements.txt

3. Run the notebook:

notebooks/deblurring.ipynb


### Google Colab (Detection and Training)
1. Upload the `data/` folder to Google Drive.
2. Open the Colab notebooks:
- `notebooks/detection_comparison.ipynb`
- `notebooks/yolo_training.ipynb`
3. Mount Google Drive in Colab and run all cells.

---

## AI Usage
AI tools were used for coding assistance, debugging, and documentation support. All prompts and outputs are recorded in:


ai_logs/prompts_and_outputs.md


This follows the assignment requirement for documenting AI usage.

---

## Git Commits
This repository uses atomic and descriptive commits to show project progress, including:
- Project setup
- Dataset preparation
- Deblurring implementation
- Detection experiments
- Dataset preparation for training
- Model fine-tuning and evaluation
- Final report and documentation
Final README Rating





