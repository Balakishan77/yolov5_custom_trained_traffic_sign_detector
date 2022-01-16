# YOLOv5 Object Detection on Traffic Signs Dataset

This notebook explains custom training of YOLOv5 model for object detection in colab using the data from Google Drive. I am using "Traffic Signs Dataset" from kaggle which is already available in yolo format.

## About this Dataset for Detection Tasks

https://www.kaggle.com/valentynsichkar/traffic-signs-dataset-in-yolo-format
This is ready to use Traffic Signs Dataset in YOLO format for Detection tasks. It can be used for training as well as for testing. Dataset consists of images in *.jpg format and *.txt files next to every image that have the same names as images files have. These *.txt files include annotations of bounding boxes of Traffic Sings in the YOLO format:

[Class Number] [center in x] [center in y] [Width] [Height]

For example, file 00001.txt includes three bounding boxes (each in a new line) that describe three Traffic Signs in 00001.jpg image:

2 0.7378676470588236 0.5125 0.030147058823529412 0.055 </br>
2 0.3044117647058823 0.65375 0.041176470588235294 0.0725 </br>
3 0.736764705882353 0.453125 0.04264705882352941 0.06875

Traffic signs in this Dataset are grouped into four categories:

1. speed limit</br>
2. yield</br>
3. mandatory</br>
4. other

## Training Custom Traffic Sign Detection Model

I have used Yolov5s for custome training with traffic sign data. I did training in Google colab by reading data from Google drive.</br> The notebook explains the below steps:
1. Setting Up Google Colab </br>
2. Cloning The YOLOv5 repository</br>
3. Mounting Google Drive</br>
4. Create traffic_sign_data.yaml (dataset config file)</br>
5. Training Custom Traffic Sign Detector Model</br>
6. Evaluate Custom YOLOv5 Detector Performance</br>
7. Run Inference With Custom YOLOv5 Object Detector Trained Weights</br>

After trainig Yolov5 on this dataset below are the some prediction results:</br>
Original image from validation set:
![image](https://user-images.githubusercontent.com/40944675/149649652-2665e49d-1167-4dc4-bb43-ca484b2d3975.png)

Inference results on the above image using Yolov5 custome trained model:
![image](https://user-images.githubusercontent.com/40944675/149649679-9af73ed1-3ba4-4525-bf58-da8bdb1fa1a9.png)



