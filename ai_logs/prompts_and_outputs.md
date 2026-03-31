# AI Prompt and Output Log – COMP6001 Assignment 1

## Entry 1 – Project Setup
Prompt:
"Help me set up the project structure, README, requirements.txt, and Git for the COMP6001 assignment."

AI Assistance:
- Suggested folder structure
- Created README template
- Created requirements.txt
- Created .gitignore
- Suggested Git workflow and commit messages

Modifications Made:
- Adjusted folder structure for Jupyter notebook workflow

Files Affected:
- README.md
- requirements.txt
- .gitignore
- notebooks/project.ipynb

Reason for Using AI:
AI was used to assist in setting up the project structure and development workflow efficiently while ensuring proper documentation and reproducibility.

## Entry 2 – Dataset Preparation and Inspection
Prompt:
"Help me correctly load matched blurred and sharp image pairs from the GoPro dataset into my assignment folders."

AI Assistance:
- Helped debug incorrect file pairing
- Suggested code to copy matched image pairs automatically
- Provided dataset inspection and visualization code

Modifications Made:
- Updated dataset paths based on local folder structure
- Limited the subset to 100 matched image pairs

Files Affected:
- notebooks/project.ipynb

Reason for Using AI:
AI was used to help prepare a clean subset of matched image pairs for quantitative and qualitative evaluation.

## Entry 3 – Deblurring and Quantitative Evaluation
Prompt:
"Help me implement image deblurring and evaluate it using PSNR, SSIM, and runtime."

AI Assistance:
- Provided a Richardson–Lucy deblurring implementation
- Provided code for PSNR and SSIM evaluation
- Helped interpret the restoration quality and computational cost

Modifications Made:
- Applied the method to a 100-image subset of the GoPro dataset
- Saved restored images and computed average evaluation metrics

Files Affected:
- notebooks/project.ipynb
- outputs/deblurring_metrics.csv
- outputs/psnr_ssim_plot.png

Reason for Using AI:
AI was used to support the development of the restoration pipeline and quantitative analysis, while all outputs were reviewed and tested manually.