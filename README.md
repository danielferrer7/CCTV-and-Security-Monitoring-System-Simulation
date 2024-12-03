# CCTV-and-Security-Monitoring-System-Simulation

Short Description of Project 3
CCTV and Security Monitoring System Simulation:
This project is a modern CCTV system built with Python, OpenCV, and Flask. It features real-time motion detection using OpenCV, logs motion events with timestamps, and displays these logs on a sleek, responsive web interface powered by Flask and Bootstrap. The system combines advanced functionality with a user-friendly, professional design.

Step-by-Step Guide of What We Did
Step 1: Set Up the Project Environment
Installed Required Libraries:
Used pip to install:
bash
Copy code
pip install flask opencv-python opencv-python-headless
Created the Folder Structure:
CCTVSystem/ (Project folder)
cctv_system.py (Main Python script)
templates/ (HTML files folder)
index.html (Web interface for logs)
Step 2: Motion Detection with OpenCV
Used OpenCV to process a live video feed:

Captured video from the webcam using cv2.VideoCapture(0).
Converted each frame to grayscale for easier processing.
Used the first frame as a reference to detect motion.
Highlighted motion with bounding rectangles by detecting differences between frames.
Logged motion events:

Recorded the timestamps of motion detections using Python's time module.
Saved the logs to a motion_log.txt file after the video feed ended.
Step 3: Created a Flask Web Interface
Set up a Flask app with a route (/) to display motion logs.
Designed a responsive HTML page (index.html) to:
Display the motion logs in a styled list.
Include a Refresh Logs button for easy log updates.
Step 4: Styled the Web Interface
Used Bootstrap 5 to style the web interface for a professional look.
Enhanced the HTML with custom CSS for gradients, hover effects, and responsive design.
