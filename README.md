# Intruder-Detection-Using-Jetson-Nano
A security system using Jetson Nano and a USB camera. Detects objects in real-time and saves a video if an intruder is detected. By using pre-trained weights and a custom dataset, the goal is to identify specific objects of interest, such as people and items, based on their appearance in surveillance footage.

## Data Used
### SOURCE:
>> COCO 2017 Dataset (Common Objects in Context)<br>
   Downloaded from: http://images.cocodataset.org

## COMPONENTS USED:
>> Annotations File: instances_train2017.json (from annotations_trainval2017.zip)<br>
>> Image Subset: Filtered from train2017 directory (original contains 118K+ images)

## Filtering Criteria:
>> Downloaded only images containing any of the following target classes (around 67,910 images):<br>
  person, backpack, handbag, suitcase, cell phone, laptop

## Model Selection
>> Selected Model: YOLOv8n (You Only Look Once v8 Nano)<br>
>> Framework: Ultralytics YOLOv8 (version 8.3.96)<br>
>> Custom Training:<br>
	- On a filtered COCO subset focused on 6 target classes:  person, backpack, handbag, suitcase, cell phone, and laptop <br>
	- Total Epochs: 50<br>
	- Image Size: 640×640<br>
	- Batch Size: 4

## EVALUATION
>> For "person", the model achieved a precision of 0.77 and a recall of 0.66, indicating that it was both accurate and consistent in detecting people<br>
>> Similarly, "laptop" showed strong detection performance with a precision of 0.72 and a recall of 0.62.<br>
>> However, the model struggled with classes like "handbag" and "cell phone“.

## FUTURE WORK
>> Live Email <br>
>> Timestamp and date for evidence<br>
>> Expanding the Model with More Class IDs







