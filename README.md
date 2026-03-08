System Architecture – Virtual Painter

The Virtual Painter system is designed to capture hand movements through a webcam and convert them into drawing actions on the screen. The architecture consists of several modules that work together to process the video input and generate the drawing output.

1. Input Module

The system uses a Webcam to capture live video of the user’s hand.

The video is divided into frames for processing.

2. Image Processing Module

The frames captured from the webcam are processed using OpenCV.

This module converts images, detects colors, and prepares the frame for hand detection.

3. Hand Detection Module

Hand landmarks are detected using MediaPipe.

It identifies finger positions and tracks hand movements.

4. Gesture Recognition Module

Based on finger positions, the system identifies gestures such as:

Drawing

Color selection

Erasing

5. Drawing Module

The drawing operation is implemented using Python.

The system maps finger movements to drawing strokes on a virtual canvas.

6. Output Module

The final drawing is displayed on the screen in real time.

Users can interact with the canvas using hand gestures.

Simple Architecture Flow
Webcam → Frame Capture → Image Processing → Hand Detection → 
Gesture Recognition → Drawing on Canvas → Display Output
