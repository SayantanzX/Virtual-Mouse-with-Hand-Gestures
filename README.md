# Virtual-Mouse-with-Hand-Gestures
This Python project allows you to control your computer mouse using hand gestures captured by your webcam. It utilizes OpenCV, MediaPipe, PyAutoGUI, and other libraries to achieve this functionality.

![Overall Trade Trend](https://github.com/SayantanzX/Virtual-Mouse-with-Hand-Gestures/blob/main/Picture.png)


Features:

Multiple Hand Detection (optional): Supports tracking and controlling the mouse with gestures from both hands.
Gesture Recognition: Detects various hand gestures for different mouse actions (click, drag, scroll, etc.).
Pinch Control for Brightness/Volume: Pinch your fingers together to adjust screen brightness or system volume.
Customizable: You can modify various parameters like hand recognition thresholds, gesture mappings, and filtering to fine-tune the experience.
Requirements:

Python 3.x
OpenCV-python
MediaPipe
PyAutoGUI
Comtypes
Pycaw
screen-brightness-control
Installation:

Clone this repository or download the ZIP file.

Install the required libraries:

Bash
pip install opencv-python mediapipe pyautogui comtypes pycaw screen-brightness-control
Use code with caution.

Usage:

Open a terminal or command prompt and navigate to the project directory.

Run the script:

Bash
python virtual_mouse.py
Use code with caution.

How it Works:

Capture Video: The script opens your webcam and captures video frames.
Hand Detection: MediaPipe's hand detection model locates hands in each frame, identifying key landmarks (fingertips, palm center).
Gesture Recognition: The HandRecog class analyzes landmark positions and finger states to determine the current hand gesture.
Mouse Control: Based on the detected gesture, the Controller class performs corresponding mouse actions using PyAutoGUI. Pinch gestures can be used to adjust system brightness or volume using the screen-brightness-control and pycaw libraries (optional).
Customization:

You can modify gesture mappings and thresholds within the HandRecog and Controller classes.
The screen-brightness-control and pycaw libraries are optional. If not installed, pinch gestures won't control brightness or volume.
Contributing:

We welcome your contributions to improve this project. Feel free to submit pull requests for bug fixes, new features, or enhancements.

License:

This project is licensed under the MIT License. See the LICENSE file for details.

Additional Notes:

For more information on OpenCV, MediaPipe, and PyAutoGUI, refer to their respective documentation.
The multiple hand detection functionality is currently disabled by default. You can uncomment the relevant sections in GestureController.classify_hands to enable it (experimental).
Consider adding more detailed instructions or comments within the code to improve readability and maintainability.
I hope this README provides a clear and informative overview of your virtual mouse project. Feel free to tailor it further based on your specific project details and preferences.
