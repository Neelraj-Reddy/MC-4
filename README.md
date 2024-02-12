Note : This project is a work in progress...

# Defect Detection in PCBs using Transfer Learning Techniques.

## Project Description
This repository contains code and resources for my research project on identifying defects in Printed Circuit Boards (PCBs). The project aims to address the growing concern of verifying PCBs as their sizes become smaller and more complex.

## Objectives
- Identify common defects in PCBs.
- Considered 6 common defects : 1-open, 2-short, 3-mousebite, 4-spur, 5-copper, 6-pin-hole.
- Develop an automated defect detection system using computer vision techniques.
- Evaluate the performance of the system on real-world datasets.

## Project Timeline
- **January 15, 2024**: Identification of the problem statement.
- **January 23, 2024**: Finalization of the dataset (DeepPCB - https://github.com/tangsanli5201/DeepPCB/tree/master.).
- **January 24 to February 2, 2024**: Exploration of various concepts and methods.
- **February 3, 2024**: Initial preprocessing and selection of YOLOv8 as the base model.
- **February 4, 2024**: First experimental run using pretrained YOLOv8 (without fine-tuning).  Overall Accuracy attained - 85 %.
- **February 8, 2024**: Creation of GitHub repository for project updates.
- **February 9, 2024**: Exploring CNN-based feature extraction to overcome alignment difference between template and defect images (Data Preprocessing).
- **February 10, 2024**: Exploring more on Feature extraction techniques.
- **February 12, 2024**: Successful implementation of the project using YOLOv8s with 11.2 million parameters. Reached accuracy of 98 %.

## Methodology
Initial Approach - We are using the YOLOv8 object detection model for defect detection in PCBs. The model is pretrained on a large dataset and then fine-tuned on our specific dataset for improved accuracy.

## Usage
To replicate our experiments, follow these steps:
1. Clone the repository.
2. Download the DeepPCB dataset.
3. Preprocess the data using the provided scripts.
4. Run the YOLOv8 model on the preprocessed data.
5. Evaluate the results and analyze the performance.

## Future Work
- Fine-tune the YOLOv8 model on our dataset for improved accuracy.
- Explore other computer vision techniques for defect detection.
- Expand the dataset to include more diverse PCB images.
