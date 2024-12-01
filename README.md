# Histopathology for Oral Cancer Diagnosis

## Overview
This project focuses on using deep learning to improve early detection and grading of oral cancer through the analysis of histopathological images. By combining advanced segmentation and classification models, the system categorizes tissue images into four severity levels: **Normal**, **Mild**, **Moderate**, and **Severe**.

## Objectives
1. Segment histopathological images to isolate relevant tissue features.
2. Classify segmented images into cancer severity levels.
3. Improve diagnostic accuracy and speed using AI techniques.

## Methodology
- **Segmentation**: Using the U-Net architecture to delineate regions in tissue samples.
- **Classification**: Employing InceptionV3 to classify segmented images into severity levels.
- **Dataset**: Includes annotated histopathology images with labeled severity.

### System Workflow
1. **Annotation**: Histopathology images are annotated with key features like hyperchromatism and pleomorphism.
2. **Segmentation**: U-Net generates masks for distinct tissue regions.
3. **Classification**: InceptionV3 categorizes the segmented images into severity levels.

![Screenshot 2024-12-02 020605](https://github.com/user-attachments/assets/3034b9b2-cdb4-4f1b-b965-8593f965217b)

## Implementation Details
### Tools and Technologies
- **Programming Language**: Python
- **Frameworks**: PyTorch
- **Deep Learning Models**: U-Net for segmentation, InceptionV3 for classification
- **Libraries**: NumPy, OpenCV, Matplotlib

### Experimental Setup
- Training performed with GPU acceleration.
- Learning rate optimization using Adam.
- CrossEntropyLoss for both segmentation and classification tasks.

## Dataset
The dataset includes histopathological images divided into four classes:
- **Normal**
- **Mild**
- **Moderate**
- **Severe**

### Dataset Statistics
| Class    | Training Samples | Testing Samples |
|----------|------------------|-----------------|
| Normal   | 127              | 37              |
| Mild     | 120              | 37              |
| Moderate | 123              | 39              |
| Severe   | 48               | 37              |

## Results
- **Segmentation Accuracy**: Improved delineation of features using U-Net.
- **Classification Accuracy**: Validation accuracy reached 56.25%.

![Screenshot 2024-12-02 020428](https://github.com/user-attachments/assets/1fd90b15-8340-4277-8900-26117a10200e)



## Future Scope
1. Integrating segmented features into classification models to improve accuracy.
2. Enhancing the segmentation module with advanced imaging techniques like hyperspectral imaging.
3. Developing a user-friendly interface for clinical deployment.

