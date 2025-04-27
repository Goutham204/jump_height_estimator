## Jump Height Estimator

This project is a Jump Height Estimator built using Python, OpenCV, MediaPipe, Tkinter, and PIL. It detects the user's jump using pose landmarks and estimates the height of the jump based on the hip position tracked over time.

How It Works:

Pose Detection: MediaPipe Pose is used to detect the human body landmarks in each video frame.

Jump Height Calculation: 

It specifically tracks the left hip landmark's y-coordinate.
At the start, the initial y-position of the hip is recorded.
While jumping, the minimum y-position is updated (the highest point of the jump).
Jump height is calculated as the difference between the initial and minimum y-values.

Video Processing:

You can use your webcam in real-time or upload a video file (.mp4, .avi) to estimate the jump height.

User Interface: 

A simple Tkinter GUI is designed with buttons to:

Start real-time video capture
Upload a pre-recorded video
Stop video
Reset the results

Libraries Used:

tkinter – for GUI
cv2 (OpenCV) – for video processing
mediapipe – for pose estimation
PIL (Pillow) – for displaying video frames inside Tkinter

