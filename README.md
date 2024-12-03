# CCTV-and-Security-Monitoring-System-Simulation

<br />
<p align="center">  
<br />
Dashboard:  <br/>
<img src="https://imgur.com/xZt4L7l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <br />
  <br />
<br />
<br />

<h2>Description</h2>
CCTV and Security Monitoring System Simulation:
This project is a modern CCTV system built with Python, OpenCV, and Flask. It features real-time motion detection using OpenCV, logs motion events with timestamps, and displays these logs on a sleek, responsive web interface powered by Flask and Bootstrap. The system combines advanced functionality with a user-friendly, professional design.


<h2>Languages and Utilities Used</h2>


- **Python**
- **OpenCV**
- **Flask**
- **Bootstrap**
- **HTML/CSS**
- **SQLite**
- **Time module**


<h2>How They Worked Together</h2>

1. **Python**:  
   The core programming language used to build the motion detection logic and integrate the web interface.

2. **OpenCV**:  
   A computer vision library used for real-time video processing and motion detection.

3. **Flask**:  
   A lightweight Python web framework used to create the web interface for displaying motion logs.

4. **Bootstrap**:  
   A front-end framework used to design a responsive and modern user interface for the web application.

5. **HTML/CSS**:  
   Used to structure and style the web pages, enhancing the UI with gradients, animations, and layouts.

6. **SQLite** (indirectly via file storage):  
   Text file storage (`motion_log.txt`) was utilized instead of a database for simplicity, simulating event logging.

7. **time module**:  
   Used to timestamp motion events, providing accurate logs of when activity was detected.

8. **VS Code or any IDE/Text Editor**:  
   A tool for writing and organizing the Python code and HTML templates.

---


<h3>Step 1: Set Up the Project Environment</h3>

1. Installed Required Libraries:
    bash
    >pip install flask opencv-python opencv-python-headless

2. Created the Folder Structure:
    >CCTVSystem/ (Project folder)
    >
    >cctv_system.py (Main Python script)
    >
    >templates/ (HTML files folder)
    >
    >index.html (Web interface for logs)

<h3>Step 2: Motion Detection with OpenCV</h3>

1. Used OpenCV to process a live video feed:

- Captured video from the webcam using cv2.VideoCapture(0).
- Converted each frame to grayscale for easier processing.
- Used the first frame as a reference to detect motion.
- Highlighted motion with bounding rectangles by detecting differences 
   between frames.

2. Logged motion events:

- Recorded the timestamps of motion detections using Python's time module.
- Saved the logs to a motion_log.txt file after the video feed ended.


<h3>Step 3: Created a Flask Web Interface</h3>

1. Set up a Flask app with a route (/) to display motion logs.
2. Designed a responsive HTML page (index.html) to:
- Display the motion logs in a styled list.
- Include a Refresh Logs button for easy log updates.


<h3>Step 4: Styled the Web Interface</h3>

1. Used **Bootstrap 5** to style the web interface for a professional look.
2. Enhanced the HTML with custom CSS for gradients, hover effects, and responsive design.


<br />
<p align="center">  
<br />
Terminal Logs:  <br/>
<img src="https://imgur.com/y4g2EyE.png" height="80%" width="80%" alt="Terminal Logs"/>
<br />
  <br />
  <br />
<br />
<br />
