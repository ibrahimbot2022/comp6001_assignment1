COMP6001 Assignment 1 – Image Restoration and Object Detection
Student Information

Name: Ibrahim Iftekhar Khan
Student ID: A1986169

Project Overview

This project investigates the effect of motion blur on object detection performance and evaluates whether image restoration (deblurring) improves detection results. The project includes image restoration, object detection experiments, dataset preparation, model fine-tuning, and performance evaluation.

Dataset

The GoPro Deblur Dataset was used in this project. The dataset contains paired blurred and sharp images captured under real motion blur conditions. Due to computational limitations, a subset of 100 matched blurred–sharp image pairs was used for the experiments.

Methods
1. Image Deblurring
Method used: Richardson–Lucy Deconvolution
Evaluation metrics:
PSNR (Peak Signal-to-Noise Ratio)
SSIM (Structural Similarity Index)
Average Results:
PSNR = 24.83
SSIM = 0.7467
2. Object Detection
Model used: YOLOv8 (Pretrained)
Detection was performed on:
Blurred images
Deblurred images
Sharp images
Detection counts and confidence scores were compared.
3. Fine-Tuning
Since the dataset did not include object detection labels, pseudo-labels were generated using YOLOv8 on sharp images.
YOLOv8 was then fine-tuned on restored (deblurred) images.
Evaluation metrics:
Precision = 0.8545
Recall = 0.4376
mAP@50 = 0.5015
mAP@50-95 = 0.3938
Repository Structure
comp6001_assignment1/
│
├── notebooks/        # Jupyter and Colab notebooks
├── outputs/          # Plots, metrics, and generated results
├── data/             # Dataset (not included in repo due to size)
├── report/           # Final report
├── slides/           # Presentation slides
├── ai_logs/          # AI usage documentation
├── README.md
├── requirements.txt
└── .gitignore
How to Run the Project
Local (Deblurring and Evaluation)
Install Python 3.10+

Install required libraries:

pip install -r requirements.txt

Run the notebook:

notebooks/deblurring.ipynb
Google Colab (Detection and Training)
Upload the data/ folder to Google Drive.
Open the Colab notebooks:
notebooks/detection_comparison.ipynb
notebooks/yolo_training.ipynb
Mount Google Drive in Colab and run all cells.
AI Usage

AI tools were used for coding assistance, debugging, and documentation support. All prompts and outputs are recorded in:

ai_logs/prompts_and_outputs.md

This follows the assignment requirement for documenting AI usage.

Git Commits

This repository uses atomic and descriptive commits to show project progress, including:

Project setup
Dataset preparation
Deblurring implementation
Detection experiments
Dataset preparation for training
Model fine-tuning and evaluation
Final report and documentation

This README now:

Explains the project clearly
Shows results
Shows how to run
Mentions AI log
Mentions Git
Mentions Colab
Looks professional