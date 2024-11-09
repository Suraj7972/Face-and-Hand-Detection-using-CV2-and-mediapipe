# Face-and-Hand-Detection-using-CV2-and-mediapipe

Real-time Facial and Hand Landmark Tracking with MediaPipe
This project demonstrates real-time facial and hand landmark detection and tracking using MediaPipe.

MediaPipe:
MediaPipe is an open-source framework built by Google for building multi-modal machine learning pipelines. It provides pre-built pipelines for tasks like pose estimation, object detection, hand tracking, and facial landmark recognition.

Project Functionality:

Captures video from your computer's default camera.
Utilizes MediaPipe's Holistic model to detect and track facial landmarks (including eyes, nose, mouth, etc.) and hand landmarks (including fingertips, knuckles, etc.) in real-time.
Visualizes the detected facial and hand landmarks on the video frame.
Calculates and displays the Frames Per Second (FPS) for performance monitoring.
Running the Project:

Requirements:

Python 3.x
OpenCV (cv2)
MediaPipe (Installation instructions)
<!-- end list -->

Install required libraries:

Bash
pip install opencv-python mediapipe
Use code with caution.

Save the code as a Python script (e.g., facial_hand_landmarks.py).

Run the script:

Bash
python facial_hand_landmarks.py
Use code with caution.

User Interaction:

Press the 'q' key to exit the application.
Code Breakdown:

Import Libraries: Imports necessary libraries like OpenCV (cv2), time, and MediaPipe's Holistic model.

Model Initialization:

Creates a Holistic instance from MediaPipe, specifying minimum detection and tracking confidence thresholds.
Initializes drawing utilities for visualizing landmarks.
Opens the default camera using OpenCV's VideoCapture.
Main Loop:

Captures frames from the camera in a loop.
Resizes the frame for better visualization.
Converts the frame from BGR to RGB for MediaPipe processing.
Runs the Holistic model on the RGB frame to detect and track landmarks.
Converts the frame back to BGR for display.
Draws facial and hand landmarks onto the frame using MediaPipe's drawing utilities.
Calculates and displays the FPS on the frame.
Displays the resulting frame with landmarks and FPS.
Waits for a key press.
Cleanup:

Releases the video capture and destroys all OpenCV windows upon termination.
Accessing Landmarks (Optional):

The commented code at the end demonstrates accessing individual landmark information from MediaPipe's HandLandmark enum.
