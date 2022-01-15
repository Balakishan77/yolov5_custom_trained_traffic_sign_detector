# yolov5_models

This notebook explains custom training of YOLOv5 model for object detection in colab using the data from Google Drive. I am using "Traffic Signs Dataset" from kaggle which is already available in yolo format.

# About this Dataset for Detection Tasks

https://www.kaggle.com/valentynsichkar/traffic-signs-dataset-in-yolo-format
This is ready to use Traffic Signs Dataset in YOLO format for Detection tasks. It can be used for training as well as for testing. Dataset consists of images in *.jpg format and *.txt files next to every image that have the same names as images files have. These *.txt files include annotations of bounding boxes of Traffic Sings in the YOLO format:

[Class Number] [center in x] [center in y] [Width] [Height]

For example, file 00001.txt includes three bounding boxes (each in a new line) that describe three Traffic Signs in 00001.jpg image:

2 0.7378676470588236 0.5125 0.030147058823529412 0.055

2 0.3044117647058823 0.65375 0.041176470588235294 0.0725

3 0.736764705882353 0.453125 0.04264705882352941 0.06875

Traffic signs in this Dataset are grouped into four categories:

prohibitory

danger

mandatory

other

Prohibitory category consists of following Traffic Signs: speed limit, no overtaking, no traffic both ways, no trucks.

Danger category consists of following Traffic Sings: priority at next intersection, danger, bend left, bend right, bend, uneven road, slippery road, road narrows, construction, traffic signal, pedestrian crossing, school crossing, cycles crossing, snow, animals.

Mandatory category consists of following Traffic Sings: go right, go left, go straight, go right or straight, go left or straight, keep right, keep left, roundabout.

Other category consists of following Traffic Sings: restriction ends, priority road, give way, stop, no entry.
