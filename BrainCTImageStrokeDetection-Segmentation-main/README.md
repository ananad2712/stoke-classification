
# BrainCTImageStrokeDetection-Segmentation
This project firstly aims to classify brain CT images into two classes namely 'Stroke' and 'Non-Stroke' using convolutional neural networks. In the second stage, the task is making the segmentation with Unet model. 

The dataset used in this project is taken from Teknofest2021-AI in Medicine competition. It contains 6000 CT images.

<h2>Detection Accuracy: %94.57 (900 Test images) | Segmentation IOU Score: %71.04 (440 Test images)<h2>


The model architecture used for the detection task: VGG16


![vgg16-1-e1542731207177](https://user-images.githubusercontent.com/56753978/134819854-bbcae054-bf93-4677-b206-dea222a6cb88.png)

The model architecture used for segmentation task: UNET


![u-net-architecture](https://user-images.githubusercontent.com/56753978/134819883-a8b284da-ff67-42de-9eff-9011f2eaa173.png)


<h2>Project includes 8 different phases:</h2>

1-Working with DICOM files, getting the images in a correct way to be able to classify/segment it easily with Deep Learning methods.

2-Creating datasets with the correct structure to use them in the project.

3-Making some required operations to images such as contouring-cropping, removing noise and centering brains to convert them into a standart format.

4-Making the operations suitable to the specific task , e.g centering is not suitable to segmentation task.

5-Making different augmentations for the two separate task.

6-Constructing the models.

7-Training/testing the models.

8-Choosing the best model.




<h2> ACCURACY VERSUS EPOCHS (visualization of accuracy over training epochs) </h2>
  

<p align="center"> 
<img src=https://user-images.githubusercontent.com/56753978/134819911-c40e90d5-5ed1-452c-9b2e-e379e5830a99.png>
  </p>


<h2>EXAMPLES</h2>
<p align="center"> 
<img src=https://user-images.githubusercontent.com/56753978/134818932-b6023adb-9eaf-4af3-9d30-d397a9ecb119.png>
</p>
  
<strong>Segmentation of hemorrhagical stroke.</strong>


<p align="center">
<img src=https://user-images.githubusercontent.com/56753978/134818936-ed268041-50c0-4f1f-bf8b-55273bdd142e.png>
</p>
  
<strong>Segmentation of ischemic stroke.</strong>
 
