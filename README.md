# SPAI-Chest-X-Ray-Pneumonia Project- Project Showcase
<p align="center">
  <img width="1250" height="300" src="https://github.com/VAIBHAVPATEL97/SPAIC-Pneumonia-Project/blob/master/project%20showcase.jpg">
</p>
This repository will contain all the necessary resources required for this project and also feel free to contribute to this repo.
There are separate folder made to update your progress of this project and to upload resources so maintain the format.

# Abstract
We have developed a model that can detect pneumonia from Chest X-Rays of the patient which has a significant level of accuracy in detecting pneumonia in comparison with practicing radiologists.  Detecting pneumonia from chest radiograph is a tough task for the radiologist. The appearance of pneumonia in X-ray images are often confusing, can overlap with other diagnoses, and can mimic many other abnormalities. So the radiologists can get confused by this, leading to waste their time as well as energy just to detect the disease like pneumonia from the radiograph. So to help them get a second opinion, they can take help of our model for the detection of pneumonia.
# Dataset
For this project, we have dataset present on kaggle.The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).

Chest X-ray images (anterior-posterior) were selected from retrospective cohorts of pediatric patients of one to five years old from Guangzhou Women and Children’s Medical Center, Guangzhou. All chest X-ray imaging was performed as part of patients’ routine clinical care.

For the analysis of chest x-ray images, all chest radiographs were initially screened for quality control by removing all low quality or unreadable scans. The diagnoses for the images were then graded by two expert physicians before being cleared for training the AI system. In order to account for any grading errors, the evaluation set was also checked by a third expert.
A glimpse of Dataset.

<p align="center">
  <img width="560" height="200" src="https://github.com/VAIBHAVPATEL97/SPAIC-Pneumonia-Project/blob/master/jZqpV51.png">
</p>

Dataset can be found on this site-https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
## Acknowledgements for this dataset
Data: https://data.mendeley.com/datasets/rscbjbr9sj/2

License: CC BY 4.0

Citation: http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5
Inspiration
Automated methods to detect and classify human diseases from medical images.
### NOTE: This dataset does not belong to us neither created by us.

# Proposed Model
#### Kaggle Kernel: 
[chest-x-ray-prediction](https://www.kaggle.com/iamsdt/chest-x-ray-prediction)

# Why RESNET101?
We have tried various other network model for this project. Below shown table shows the comparision of various models and their effect of the accuracy of prediction.

| Model Name  | Accuracy of class 1- Pneumonia detected |Accuracy of class 2- Pneumonia is not detected|
| ------------- | ------------- |  ------------- |
| VGG16  | Content Cell  | |
| RESNET 51  | Content Cell  ||
| RESNET 101  | Content Cell  ||
# About RESNET101.
[Paper on RESNET by arvix](https://arxiv.org/pdf/1512.03385.pdf)
We used transfer learning Method
And used Resnet101 pretrained model

# Model Architecture

CNN layers: <br>
Linear Layer: 3 layers<br>
Pooling: LogSoftmax<br>
Activation Function: Mila<br>

# Hyper parameters
Batch size: 32
Learning rate:0.0001<br>
Optimizer:Rectified Adam (RAdam)<br>
Loss function:Cross Entropy <br>
Epoch: 10 <br>
Transformation:<br>

# Accuracy


Total Accuracy:<br>
Class wise accuracy:<br>


### Libraries version
Prerequisite packages which should be there in your run environment to run this project model.

| Package Name  | Version Number |
| ------------- | ------------- |
| Torch  | 1.2.0  |
| Torch vision  |  0.4.0a0+6b959ee|
| Numpy | 1.17.0 |
|Matplotlib  | 3.0.3 |
| PIL  | 5.4.0 |

## Contributors of this project are:

| Name | Slack Name |
| --- | ---|
| Vaibhav Patel| Vebby
| Shudipto Trafder | Shudipto Trafder
| Sankalp Dayal | Sankalp Dayal


# References 
[CheXNet: Radiologist-Level Pneumonia Detection on Chest X-Rays with Deep Learning](https://stanfordmlgroup.github.io/projects/chexnet/)

[Can Machine Learning Read Chest X-rays like Radiologists?](https://towardsdatascience.com/can-machine-learning-read-chest-x-rays-like-radiologists-part-1-7182cf4b87ff)

[Effecient Deep Network Architectures for Fast Chest X-Ray Tuberculosis Screening and Visualization](https://www.nature.com/articles/s41598-019-42557-4.pdf)


[ChesXNET by stanford](https://arxiv.org/pdf/1711.05225.pdf)
