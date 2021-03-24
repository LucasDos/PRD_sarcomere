# Projet de Recherche et Développement
#### Mesure multiple et rapide de sarcomère
###### Etudiant : Dos Santos Lucas
###### Tuteur académique : Donatello Conte

## Installation
Dans un premier temps, il faut installer les librairies nécessaire afin d'executer la détection avec Yolov5.
```bash
cd /yolov5
pip install -r requierements.txt
```

## Setup avant détection

1. Déplacer les vidéos

```bash
cd /yolov5
python detect.py --weights runs/custom_models/yolov5_s-16-150.pt --img 416 --conf 0.4 --source ../data_to_detect
```


