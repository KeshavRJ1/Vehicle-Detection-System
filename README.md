🚗 Vehicle Detection System using OpenCV
A robust computer vision solution designed to detect and track moving vehicles in pre-recorded traffic video streams. This project leverages classical image processing techniques to identify regions of interest and visualize vehicle movement with bounding boxes. 

📋 Table of Contents
Project Overview
Key Features
How It Works
Tech Stack
Future Enhancements

📌 Project Overview
Monitoring traffic flow is essential for smart city infrastructure. This system provides a lightweight alternative to heavy deep learning models by using Background Subtraction and Contour Analysis to detect vehicles in recorded video clips. It is ideal for traffic analysis where computational resources are limited. 

✨ Key Features
Dynamic Detection: Identifies moving vehicles while ignoring static backgrounds.
Real-time Visualization: Draws automated bounding boxes around detected objects.
Preprocessing Pipeline: Includes Gaussian Blur and Dilation to reduce noise and improve accuracy.
Lightweight Performance: Runs efficiently on standard CPUs without requiring a GPU. 

⚙ How It Works
The system follows a structured computer vision pipeline: 
Frame Preprocessing: Converts video frames to grayscale and applies a Gaussian Blur to remove high-frequency noise.
Background Subtraction: Uses the MOG2 or KNN subtractor to isolate moving objects from the static road.
Morphological Operations: Applies Dilation to close gaps in detected "blobs," ensuring vehicles are seen as single solid objects.
Contour Detection: Finds the boundaries of the moving blobs.
Filtering & Labeling: Filters out small contours (like shadows or birds) and draws rectangular bounding boxes around legitimate vehicles. 

🛠 Tech Stack
Language: Python
Library: OpenCV (Open Source Computer Vision Library)
Mathematical Operations: NumPy
Environment: Python 3.x .

🔮 Future Enhancements
Vehicle Counting: Implement a "crossing line" logic to count how many vehicles pass a specific point.
Classification: Integrate a pre-trained Haar Cascade or YOLO model to distinguish between cars, trucks, and motorcycles.
Speed Estimation: Calculate vehicle speed based on frame rate and pixel displacement.
Cloud Logging: Export traffic data to a CSV or database for long-term analysis. 


Developed by
Keshav Joshi
