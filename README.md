# SoundWave

This project uses hand gestures to control the system volume. The implementation uses OpenCV for video capture and processing, MediaPipe for hand tracking, and PyAutoGUI for simulating keyboard presses.

## How It Works

The system detects the positions of the thumb tip and the index fingertip using MediaPipe. By calculating the distance between these two points, the system determines whether to increase or decrease the volume.

- **Thumb Tip (ID 4)**
- **Index Fingertip (ID 8)**

If the distance between the thumb tip and the index fingertip is greater than a threshold, the volume is increased. Otherwise, the volume is decreased.

## Requirements

- Python 3.x
- OpenCV
- MediaPipe
- PyAutoGUI

## Installation

Install the required packages:

```sh
pip install opencv-python mediapipe pyautogui

