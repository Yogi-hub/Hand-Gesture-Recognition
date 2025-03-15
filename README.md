# Hand Gesture Recognition using OpenCV

This project implements a real-time hand gesture recognition system using OpenCV and Python. The system detects hand gestures using contour and convex hull techniques. It dispays the equivalent numeric value (1 to 5) as depicted by the hand gesture, based on number of fingers raised.

## Features

- Uses OpenCV to capture and process video from a webcam.
- Detects hand region using HSV color segmentation.
- Identifies contours and convex hulls to recognize hand gestures.
- Counts the number of fingers raised and displays corresponding gesture labels.
- Provides real-time feedback on screen.

## Requirements

Make sure you have the following dependencies installed:

```bash
pip install opencv-python numpy
```

## Usage

Run the script using:

```bash
python hand_gesture_recognition.py
```

Press `Esc` to exit the application.

## How It Works

1. Captures video feed from the webcam.
2. Defines a region of interest (ROI) where hand gestures are detected.
3. Converts the ROI to HSV color space and applies a mask to detect skin color.
4. Finds the contours of the hand and creates a convex hull.
5. Calculates convexity defects to determine the number of fingers raised.
6. Displays the recognized gesture on the screen.

## Supported Gestures

- **0 Fingers**: No fingers raised.
- **1 Finger**: Index finger raised.
- **2 Fingers**: Two fingers raised.
- **3 Fingers**: Three fingers raised.
- **4 Fingers**: Four fingers raised.
- **5 Fingers**: All fingers raised.
- **OK Sign**: Recognized when specific convexity defect conditions are met.
- **Best of Luck Sign**: Special gesture recognition based on area ratio.

## Author

D. Yokesh

## License

This project is open-source and available under the MIT License.


