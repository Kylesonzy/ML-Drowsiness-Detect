# ML-Drowsiness-Detection
Monitors a driver’s eyes in real time to assess if they are open or closed.

# How It's Built
Technologies Used: YOLOv5, OpenCV, PyTorch, Python, Jupyter Notebooks

This project performs real-time object detection using the COCO (Common Objects in Context) dataset to detect human faces and determine whether the eyes are open or closed. OpenCV is employed to capture real-time video frames, which are then processed by a YOLOv5-trained model for face and eye state detection.

The main functionality revolves around a loop that continuously captures frames from the webcam, runs detections on those frames, and renders the results. This loop remains active until the user presses 'q' to quit the application.

# Optimizations
Various optimizations were applied to ensure efficient and real-time performance. The frame capture and rendering processes were streamlined to eliminate lag, ensuring that real-time detections are displayed without delay. The model was also fine-tuned to achieve accurate detections while minimizing false positives/negatives. Efficient loading of assets and models was prioritized to ensure fast startup times and quick responsiveness.

# Lessons Learned
Balancing Accuracy and Performance: A key takeaway from this project was finding the right balance between detection accuracy and real-time performance. This required repeated iterations, testing, and tuning to ensure the model was both precise and responsive.

Integration Challenges: Combining different technologies such as OpenCV, PyTorch, and YOLOv5 posed integration challenges, underscoring the importance of understanding how various libraries and frameworks interact with each other.

# Acknowledgements
Special thanks to the open-source community for providing invaluable resources, libraries, and frameworks that were crucial to the development of this project. The contributions of developers from YOLOv5, OpenCV, and PyTorch were particularly instrumental in bringing this project to completion.
