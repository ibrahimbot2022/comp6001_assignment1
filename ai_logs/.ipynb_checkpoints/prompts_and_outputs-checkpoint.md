# AI Prompt and Output Log – COMP6001 Assignment 1

## AI Usage Statement

AI tools were used as a coding assistant, debugging assistant, and for guidance on experiment design and result interpretation. 
All code was reviewed, modified, and executed by me. 
All experiments, model training, evaluations, and report writing were performed by me. 
AI was not used to generate results, and all results reported in this project were obtained through actual experiments conducted by me .

Entry 1 – Project Setup

Prompt:
"set up the project structure, README, requirements.txt, and Git for the COMP6001 assignment."

AI Assistance:
AI suggested a suitable folder structure, helped create a README template, requirements.txt, and .gitignore file, and explained how to use Git with proper commit messages.

Modifications Made:
The folder structure was slightly modified to support a Jupyter notebook workflow instead of only Python scripts.

Files Affected:

README.md
requirements.txt
.gitignore
notebooks/project.ipynb

Reason for Using AI:
AI was used to help set up the project structure and workflow correctly at the beginning of the project.

Entry 2 – Dataset Preparation and Inspection

Prompt:
"correctly load matched blurred and sharp image pairs from the GoPro dataset into my assignment folders."

AI Assistance:
AI helped debug incorrect file pairing and suggested code to automatically copy matched blurred and sharp image pairs. It also provided code to inspect and visualize the dataset.

Modifications Made:
Dataset paths were updated based on the local system and a subset of 100 matched image pairs was selected for experimentation.

Files Affected:

notebooks/project.ipynb

Reason for Using AI:
AI was used to help prepare a clean and correctly matched dataset for evaluation and experiments.

Entry 3 – Deblurring and Quantitative Evaluation

Prompt:
"implement image deblurring and evaluate it using PSNR, SSIM, and runtime."

AI Assistance:
AI provided a Richardson–Lucy deblurring implementation and helped with code to calculate PSNR and SSIM. AI also helped explain how to interpret these metrics.

Modifications Made:
The method was applied to a subset of 100 images and the restored images and evaluation results were saved.

Files Affected:

notebooks/project.ipynb
outputs/deblurring_metrics.csv
outputs/psnr_ssim_plot.png

Reason for Using AI:
AI was used to assist with implementing the restoration method and evaluation metrics.

Entry 4 – Object Detection Comparison

Prompt:
"run YOLOv8 object detection on blurred, deblurred, and sharp images and compare detection results."

AI Assistance:
AI helped with YOLOv8 inference code, counting detections, calculating average confidence scores, and identifying failure cases.

Modifications Made:
Detection was run on blurred, restored, and sharp images, and the results were saved as plots and tables for analysis.

Files Affected:

notebooks/object_detection_comparison.ipynb
outputs/detection_comparison_plots.png

Reason for Using AI:
AI was used to help set up the object detection experiments and analyse the results.

Entry 5 – Pseudo-Label Generation and Dataset Preparation

Prompt:
" generate pseudo-labels using a pre-trained YOLO model and prepare the dataset for training."

AI Assistance:
AI helped with generating pseudo-labels from sharp images, converting them into YOLO annotation format, splitting the dataset into training and validation sets, and creating the data.yaml file.

Modifications Made:
Paths were adjusted for Google Colab and the dataset structure was created for training.

Files Affected:

notebooks/yolo_training.ipynb
yolo_dataset/images/train
yolo_dataset/images/val
yolo_dataset/labels/train
yolo_dataset/labels/val
yolo_dataset/data.yaml

Reason for Using AI:
AI was used to help prepare the dataset in the correct format for YOLO training.

Entry 6 – YOLO Fine-Tuning and Evaluation

Prompt:
"fine-tune YOLO on restored images and evaluate the model using precision, recall, and mAP."

AI Assistance:
AI helped with training code, suggested training parameters, and helped explain the evaluation metrics and results.

Modifications Made:
An initial YOLOv8n model was trained, followed by a stronger YOLOv8s model with more epochs and data augmentation. The results were then compared.

Files Affected:

notebooks/yolo_training.ipynb
outputs/training_results.txt
outputs/final_detection_comparison.png

Reason for Using AI:
AI was used to assist with training setup and understanding the evaluation results.