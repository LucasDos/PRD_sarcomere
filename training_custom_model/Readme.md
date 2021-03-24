# Training custom detection model


### Roboflow : Create custom dataset 
Site : [Roboflow](https://app.roboflow.com/)

--- 
&nbsp;
#### Create dataset

First, to train our custom detection model, we need to create our own dataset of images. 
In this project I create a sarcomere dataset.

![alt text](https://drive.google.com/uc?export=view&id=1cD4hq9yRuyKLFiLOEIcO3EQnCBTeNzz_)

* Dataset Type : choose Object bounding (Bouding box)
* Annotation Group : for this project I have one class **sarc** but you can define other classes with "," separator. If you forgot classes, you can add them later.

--- 
&nbsp;
#### Uploading your own images

![alt text](https://drive.google.com/uc?export=view&id=1UO27FiOJIv6qZnFcWwTee4ryJole9G24)

After uploading your images, roboflow proposed to split your data into three parts :
* Train : This is the number of training images. The model will train on this set.
* Valid : This is the number of valid images. The model will use it during the training to evaluate is precision.
* Test : This is the number of test images. This set is for after training to verify if your model is efficient or not.

--- 
&nbsp;
#### Classify your images

Now you can classify your images with bounding box and your different classes by clicking on an image.

![alt text](https://drive.google.com/uc?export=view&id=1FRCXqUwCa0EMQMeQERyfXorssXsrmgcr)

--- 
&nbsp;
#### Generate your dataset
Once the previous step is completed you can download or export your dataset to use it on YOLO v5 by clicking on generate.

![alt text](https://drive.google.com/uc?export=view&id=1kD-Zit4JR-s2fuQQK257IX62jGqQuJCQ)

* Choose **YOLO v5 PyTorch** in the drop down menu
* Choose **download zip** or **download code** (in this project we choose download code to use it with Google Colaboratory).

Now you can generate your final dataset and use it on YOLO v5 project.
![alt text](https://drive.google.com/uc?export=view&id=1NavnfKnUN0hoK8yi196hDZdwhBihlf3w)

--- 
&nbsp;
#### Google Colaboratory : Training our custom model

Now that we have our custom dataset, we can open **training_custom_dataset.ipynb** on Google Colaboratory.
All the step are explain directly on this file.

###### *Sources*
*[Yolo v5](https://github.com/ultralytics/yolov5)*

*[Train custom dataset](https://blog.roboflow.com/how-to-train-yolov5-on-a-custom-dataset/)*

