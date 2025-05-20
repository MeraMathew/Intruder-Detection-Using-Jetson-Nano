# Intruder-Detection-Using-Jetson-Nano
A security system using Jetson Nano and a USB camera. Detects objects in real-time and saves a video if an intruder is detected. By using pre-trained weights and a custom dataset, the goal is to identify specific objects of interest, such as people and items, based on their appearance in surveillance footage.

##Data Used
###SOURCE:
COCO 2017 Dataset
Common Objects in Context
Downloaded from: http://images.cocodataset.org
![image](https://github.com/user-attachments/assets/be4ebef4-5407-4f35-853c-340b5721aae0)

##COMPONENTS USED:
Annotations File: instances_train2017.json (from annotations_trainval2017.zip)
Image Subset: Filtered from train2017 directory (original contains 118K+ images![image](https://github.com/user-attachments/assets/b5c13bb3-f68c-4702-a13d-d1062471c575))

##Filtering Criteria:
Downloaded only images containing any of the following target classes (around 67,910 images):
person, backpack, handbag, suitcase, cell phone, laptop
![image](https://github.com/user-attachments/assets/ca99e634-c1e5-4736-a2fc-c3fe916a0912)


