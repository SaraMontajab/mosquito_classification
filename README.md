# Mosquito Classification

### Final Project for ENSF 619.2:

DEEP LEARNING ARCHITECTURES EVALUATION FOR CLASSIFICATION OF MOSQUITO SPECIES ALONG WITH MODEL INTERPRETATION USING GRADCAM

## Introduction

Mosquitoes, known for spreading deadly diseases worldwide, are a global health challenge. The identification of mosquito species is crucial for controlling the spread of these diseases. Leveraging the advancements in deep learning, this study demonstrates that mosquito species can be accurately identified through images captured by standard cameras, bypassing the need for microscopic examination. Our evaluation focused on deep learning models, with a particular emphasis on the application of the Grad-CAM method to enhance model transparency. This approach not only achieved an impressive accuracy in classifying 650 mosquito images across five species (Aedes, Bandar, Chabahar, Kazeron, Culex) but also provided valuable visual insights into the decision-making processes of the models, shedding light on the distinguishing features used for species classification. This research marks a significant step forward in the use of machine learning for public health surveillance and mosquito-borne disease control.


## Dataset

Our dataset we used 650 mosquito images with distribution of 80% and 20% for the training and testing sets. 
[Dataset Link](https://drive.google.com/drive/folders/1_xQgT1jGbqhdrX6sISamVRJWdGxV8NH4?usp=drive_link)

## Our Approach

- Classification of 5 species of mosquitos namely: Aedes, Bandar, Chabahar, Kazeron, Culex  

- Using dataset with 650 images to show the models predictions on small dataset

- Using 5 Deep Learning (DL) models: DenseNet121, ResNet-18, ResNet-50, VGG-16, AlexNet

- Using Grad-CAM to get the interpretation of the DL models used


## Results

### Evaluation Results

| Deep Learning Models | Train Accuracy (%) | Test Accuracy (%) | Train Time (s) | Precision | Recall | F1-Score |
| -------------------- | ------------------ | ----------------- | -------------- | --------- | ------ | -------- |
| DenseNet121 | 79.8 | 67.3 | 915 | 0.78 | 0.73 | 0.72 |
| ResNet18    | 79.5 | 73.4 | 826 | 0.81 | 0.76 | 0.73 |
| ResNet50    | 75.3 | 73.4 | 788 | 0.86 | 0.76 | 0.72 |
| VGG16       | 64   | 63.2 | 896 | 0.85 | 0.73 | 0.68 |
| AlexNet     | 68.6 | 69.3 | 921 | 0.73 | 0.67 | 0.67 |


### Grad-CAM Results

The results show that ResNet18 and ResNet50 have the best results based on the visualization given by Grad-CAM. From left to right the images are: original, Grad-CAM visualization, and Grad-CAM++ visualization.

![grad-cam](img/grad-cam.png)


## Conclusion

- ResNet18 and ResNet50 models performed best in classifying mosquito species from a small dataset.

- VGG16 and AlexNet did not perform as efficiently, highlighting the advantages of newer models with limited data.

- Grad-CAM visualizations provided clear insights into the reasoning behind the models' classifications. The models focused on key mosquito features like the thorax and wings, crucial for correct species identification.

