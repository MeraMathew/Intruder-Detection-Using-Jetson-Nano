# Intruder-Detection-Using-Jetson-Nano
A security system using Jetson Nano and a USB camera. Detects objects in real-time and saves a video if an intruder is detected. By using pre-trained weights and a custom dataset, the goal is to identify specific objects of interest, such as people and items, based on their appearance in surveillance footage.

## Data Used
### SOURCE:
COCO 2017 Dataset
Common Objects in Context
Downloaded from: http://images.cocodataset.org

## COMPONENTS USED:
Annotations File: instances_train2017.json (from annotations_trainval2017.zip)
Image Subset: Filtered from train2017 directory (original contains 118K+ images)

## Filtering Criteria:
Downloaded only images containing any of the following target classes (around 67,910 images):
person, backpack, handbag, suitcase, cell phone, laptop



