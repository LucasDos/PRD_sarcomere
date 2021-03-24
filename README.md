# Search & Development Project 
#### *Multiple and fast sarcomere measurement*
###### *Student : Dos Santos Lucas*
###### *Academic Supervisor : Donatello Conte*
![alt text](https://drive.google.com/uc?export=view&id=1H_fksBZue4YevwIYFWQ8kVQoYg4UVCEN)

## Installation
First of all it's necessary to install the libraries for running the Yolov5 detection model.
Go to the folder **/yolov5** and run the following command :
```bash
$ pip install -r requierements.txt
```

## Détection
* **Setup**

Copy your data *(images/videos)* in the **/data_to_detect** folder. The detection will be done on this data.

* **Run detection**

To run the detection, goto the folder **/yolov5** and run the following command :
```bash
python detect.py --weights custom_models/yolov5_s-16-150.pt --img 416 --conf 0.4 --source ../data_to_detect
```

* **Results**

Finally, the results are saved in **/run/detect/exp{num_exp}** folder and you can consult them when you want.

![alt text](https://drive.google.com/uc?export=view&id=1ezOcnnQNyYXimPNHacGg8mOoDfORDvtj)

## Entraîner un modèle personalisé

Pour entrainer un modèle personnalisé, il suffit d'ouvrir le fichier **training_custom_model.ipynb** via Google Colaboratory et suivre les étapes.

###### *Sources*
*[Yolo v5](https://github.com/ultralytics/yolov5)*

*[Train custom dataset](https://blog.roboflow.com/how-to-train-yolov5-on-a-custom-dataset/)*

