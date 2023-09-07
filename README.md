# Object-Tracking-PyTorch-YOLOv5-DeepSort

This repo represents implimentation of YOLOv5 and DeepSort in Pytorch for object tracking


![Demo](img.gif)

# Information
DeepSORT is an advanced object tracking algorithm that leverages deep learning for feature extraction and combines it with traditional tracking techniques to provide robust and accurate multi-object tracking. It effectively addresses many of the challenges in object tracking, making it suitable for a wide range of applications.



DeepSORT Overview: DeepSORT (Deep Learning-based Object Tracking with Re-Identification) is a powerful object tracking algorithm that combines deep learning and traditional tracking methods for accurate multi-object tracking.

Feature Extraction: Instead of explicitly detecting key points, DeepSORT extracts deep features from objects, using convolutional neural networks (CNNs) to represent object appearances effectively.

Feature Matching: DeepSORT uses these deep features to match objects across frames, associating them with existing tracks. This enables it to handle challenges like occlusions and scale changes.

Motion Estimation: DeepSORT estimates object motion by predicting future locations based on past positions and velocities, often incorporating Kalman filtering for improved accuracy.

Applications: DeepSORT is applied in real-time scenarios such as video surveillance, crowd monitoring, autonomous vehicles, and more, where robust and precise multi-object tracking is crucial.

# How to Run the project 
1.Clone the respo : 
git clone
2.create virtual environment in local machine 
conda create -p venv python==3.7 -y
3.Install python packages
pip install -r requirements.txt
4. Run the command
python detect_sort.py --weights yolov5s.pt  --img 640  --source pedestrian.mp4
5.For web camera detection 
python detect_sort.py --weights yolov5s.pt  --img 640  --source 0


