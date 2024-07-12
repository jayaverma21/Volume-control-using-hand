# Volume Control with Hand Gestures
This project demonstrates how to control the system volume using hand gestures with OpenCV, the HandTrackingModule from cvzone, and pyautogui. By using computer vision techniques, the project tracks the user's hand in real-time and adjusts the system volume based on the distance between the thumb and index finger. This allows for an intuitive and touchless way to control volume, enhancing user experience and accessibility.

# Features
+ Real-time Hand Detection: Utilizes the webcam to detect hands in real-time.
+ Gesture Recognition: Specifically tracks the thumb and index finger to determine their distance.
+ Volume Control: Adjusts the system volume based on the distance between the thumb and index finger.
+ Visual Feedback: Displays the current volume level on the video feed.
+ Cross-Platform: Works on different operating systems thanks to the pyautogui module.

# Requirements
+ Python 3.x
+ OpenCV: For video capture and image processing.
+ numpy: For numerical operations.
+ cvzone: For simplified hand detection using the HandTrackingModule.
+ pyautogui: For controlling the system volume.

# Installation
```pip install opencv-python numpy cvzone pyautogui```


# Usage
Run the following command to start the application:
```python volume_control_hand_gesture.py```

# Code Explanation
The main script volume_control_hand_gesture.py does the following:

+ Initializes the HandDetector from the cvzone module with a detection confidence of 0.8.
+ Captures video from the webcam.
+ Detects hands and landmarks in each frame.
+ Calculates the distance between the tips of the thumb and index finger.
+ Maps this distance to a volume level.
+ Uses pyautogui to adjust the system volume based on the hand gestures.
+ Ends the application when the 'q' key is pressed.
