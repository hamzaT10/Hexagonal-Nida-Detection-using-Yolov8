# Hexagonal-Nida-Detection-using-Yolov8
# Project Overview
The Hexagonal Nida Detection using YOLOv8 project is designed to detect and localize hexagonal patterns in honeycomb structures with high precision. This project is primarily aimed at improving CNC machine automation, where the detected hexagonal shapes are used to guide the machine to accurately cut the center of each side of the hexagons. These precise cuts are critical in industries such as aerospace, automotive, and manufacturing, where honeycomb structures are used for lightweight, yet durable materials.

By leveraging the powerful YOLOv8 object detection model, this project ensures that the hexagonal patterns can be detected in real-time, and the exact trajectory for cutting is calculated, facilitating automated and precise machining processes.

# Key Features
Hexagonal Pattern Detection: Uses YOLOv8 to detect hexagonal shapes in complex honeycomb structures, providing accurate data for CNC machine guidance.
Automated CNC Trajectory: Outputs the center points of each hexagonal side, enabling automated cutting by CNC machines.
Custom Dataset: A dataset of honeycomb structures was annotated and preprocessed to train the YOLOv8 model for high-accuracy detection.
Real-time Detection: Enables real-time processing for industrial applications where speed and precision are critical.
Scalability: Designed to work in various environments and with different hexagonal configurations, making it adaptable to diverse industrial needs.
# Technologies Used
YOLOv8: The state-of-the-art object detection model used for detecting hexagonal patterns and generating CNC cutting paths.
Python: Main programming language for developing the detection model and CNC trajectory calculation.
Roboflow: Used for annotating and augmenting the dataset to train the YOLOv8 model.
OpenCV: Applied for image processing and calculating precise cut points for CNC operations.
PyTorch: Framework used for training and fine-tuning the YOLOv8 model.
NumPy & Matplotlib: Used for data manipulation and visualization.
# Purpose of the Project
The primary goal of this project is to automate the cutting process of hexagonal honeycomb structures using a CNC machine. By detecting the hexagonal patterns and calculating the center of each side, the project provides an efficient way to define the cutting trajectory, ensuring precise and automated cuts for industrial applications. This improves both the speed and accuracy of CNC operations, reducing manual labor and enhancing production quality.

# Dataset
The dataset consists of high-resolution images of honeycomb structures annotated for hexagonal shapes. Roboflow was used for annotation and data augmentation, including transformations like rotation, scaling, and flipping, to ensure robust detection under different conditions. The dataset was crucial for training YOLOv8 to accurately identify hexagonal shapes and extract the necessary geometric data for CNC trajectory calculations.

# Model Training
The YOLOv8 model was fine-tuned using a pre-trained model as a base, and trained on the custom dataset to detect hexagonal patterns. During training, the model learned to identify hexagons and output the coordinates required for cutting the centers of their sides with high precision. Evaluation metrics like precision, recall, and mean Average Precision (mAP) were used to measure the model's effectiveness.

# Results
The model accurately detects hexagonal patterns and outputs the exact points needed for CNC machine cutting. The results show high precision in real-time detection, even in complex and cluttered environments. The trajectory for cutting the center of each hexagon side was generated efficiently, ensuring optimal automation for CNC machines.
