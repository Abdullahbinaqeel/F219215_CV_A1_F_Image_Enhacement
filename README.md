# F219215_CV_A1_F_Image_Enhacement
#Image Enhacement for dull and dark Brain tumor images for better and clear results.
#Image Enhancement 

##Overview
This project addresses the real-world problem of enhancing low-contrast Magnetic Resonance Imaging (MRI) scans of the human brain. The primary goal is to improve the visibility of brain tumors, which are often difficult to distinguish from healthy tissue in raw MRI images.

##Problem
Radiologists and medical professionals often face challenges in accurately identifying tumor boundaries in low-contrast MRI scans. This project aims to apply image enhancement techniques to increase the clarity and detail of these images, thereby aiding in more precise diagnosis and treatment planning.

##Methodology
The solution combines two key image processing techniques:

##Histogram Equalization: Used as a foundational step to improve the overall global contrast of the image. This method spreads out the pixel intensity values to create a more uniform histogram, revealing details that were previously hidden.

##Gamma Correction: Applied after histogram equalization to fine-tune the tonal response of the image. A gamma value of less than 1.0 is used to brighten the darker regions, further highlighting subtle details within the tumor and its surroundings.

##Dataset
The project utilizes the Brain Tumor MRI Dataset from Kaggle, accessed programmatically via the kagglehub library. This dataset provides a suitable collection of images that benefit from contrast enhancement.

##Requirements
To run the provided Python script, you need to have the following libraries installed:
opencv-python
numpy

##Usage
The core functionality is contained within the enhance_mri.py script. To run the script, use the following command in your terminal, replacing <path_to_image> with the path to the MRI image you wish to enhance:

python enhance_mri.py <path_to_image>

The script will save the enhanced image in the same directory with a prefix of enhanced_.
