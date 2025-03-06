# Gesture-Control-Mouse-

Gesture Control Mouse using Computer Vision

Description
This project implements a virtual mouse using hand gestures, leveraging computer vision and machine learning. It uses OpenCV, MediaPipe, and PyAutoGUI to track hand movements and simulate mouse actions.

Features
- Hand Tracking: Uses MediaPipe Hands to detect and track hand movements in real-time.
- Cursor Control: Moves the cursor based on the index finger's position.
- Click Detection: Detects thumb-index finger pinch gestures to perform left clicks.
- Smooth Movement: Maps hand coordinates to screen coordinates for smoother control.
- Click Optimization: Uses Euclidean distance-based thresholding to detect clicks while preventing accidental rapid clicks.
- Future Enhancements:
  - Right-click and scrolling functionality.
  - Multi-finger gestures for additional controls.
  - Adjustable sensitivity and dynamic thresholds.

Technologies Used
- Programming Language: Python
- Libraries:
  - OpenCV (Computer Vision)
  - MediaPipe (Hand Tracking)
  - PyAutoGUI (Mouse Control)
  - NumPy (Numerical Computation)
  - Time (Delay Handling)

Installation
1. Install dependencies:
   pip install opencv-python mediapipe pyautogui numpy

2. Run the program:
   python gesture_mouse.py

Usage
- Move the cursor: Move your index finger in the air.
- Left Click: Pinch your thumb and index finger together.
- Right Click & Scroll (Future Work): Additional gestures can be implemented.

How It Works
1. Hand Tracking:
   - Uses MediaPipe Hands to detect hand landmarks.
   - Extracts the index finger tip and thumb tip positions.

2. Cursor Movement:
   - Maps hand coordinates to screen coordinates.
   - Uses a scaling factor for smoother control.

3. Click Detection:
   - Calculates Euclidean distance between thumb and index finger.
   - If the distance is below a certain threshold, a click event is triggered.

4. Optimization:
   - Implements delay handling to prevent accidental multiple clicks.
   - Adjusts sensitivity and thresholds dynamically.

Project Structure
/gesture-control-mouse
│── gesture_mouse.py       # Main Python script
│── requirements.txt       # List of dependencies
│── README.md              # Project Documentation


Future Improvements
- Implement right-click and scrolling gestures.
- Optimize movement smoothing and accuracy.
- Add UI elements to configure sensitivity settings.

Contributors
- Gunjan Raghav

