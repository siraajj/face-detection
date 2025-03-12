# Real-Time Face Detection with OpenCV

This project demonstrates real-time face detection using OpenCV and Haar Cascade Classifiers. The program captures video from the default camera and detects faces, drawing bounding boxes around them. It uses the `haarcascade_frontalface_default.xml` classifier provided by OpenCV.

## Features

- Real-time face detection.
- Draw bounding boxes around detected faces.
- Utilizes the default webcam to capture live video.
- Press 'q' to exit the video feed.

## Requirements

Before running the code, make sure to install the required dependencies:

- Python 3.x
- OpenCV

You can install OpenCV using pip:

```bash
pip install opencv-python
```
## How to Run
1. Clone the repository:
```
git clone https://github.com/sirajj/face-detection.git
cd face-detection
```
2. Run the Python script:

```
python face_detection.py
```
3. The program will open a window showing the live video feed with bounding boxes around detected faces. Press 'q' to close the window and stop the program.
## Code Overview
`face_detection.py`

1. **Loading the Classifier:** The program loads the pre-trained face detection model `haarcascade_frontalface_default.xml` from OpenCV.

2. **Capture Video Feed:** The script captures the video from the webcam using OpenCV's `cv2.VideoCapture(0)` function.

3. **Face Detection:** The `detect_bounding_box()` function converts the captured frame to grayscale and applies the Haar Cascade classifier to detect faces. The faces are then highlighted with green rectangles.

4. **Exit:** Press 'q' while the video feed is displayed to exit the program.

## Example Output
The program displays the webcam feed with bounding boxes around any detected faces.


## Troubleshooting
- If the webcam does not work or gives an error, ensure that your system has the correct drivers installed for the camera.
- If OpenCV is not installed, you can install it via pip install opencv-python.
## License
This project is licensed under the MIT License - see the LICENSE file for details.