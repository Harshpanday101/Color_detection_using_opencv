# Object Detection Using OpenCV

This project detects a specific color object in a video stream using **OpenCV** and **PIL (Pillow)**. It captures live video from the webcam, processes frames to detect objects of a specified color, and highlights them with a bounding box.

## Features
- Detects objects of a particular color in real-time.
- Uses OpenCV for image processing.
- Uses PIL to get object bounding boxes.
- Live video feed with color-based object tracking.

## Project Structure
```
├── main.py             # Main script to run the object detection
├── util.py             # Utility functions for color range conversion
├── requirements.txt    # List of dependencies
└── README.md           # Documentation
```

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/Harshpanday101/Color_detection_using_opencv.git
cd Color_detection_using_opencv
```

### 2. Install Dependencies
Ensure you have Python installed (recommended: Python 3.7+). Install the required libraries using:
```bash
pip install -r requirement.txt
```

## Usage
Run the following command to start the object detection:
```bash
python main.py
```

### How It Works
1. Captures video from the webcam.
2. Converts frames to HSV color space.
3. Applies a mask to filter the specified color.
4. Detects the object's bounding box and draws a rectangle around it.
5. Press **'q'** to exit the application.

## Dependencies
The required dependencies are listed in `requirements.txt`. They include:
- **OpenCV** (`cv2`) – Image processing and video capture.
- **Pillow (PIL)** – Used for bounding box detection.
- **NumPy** – Numerical operations.

## Customization
- Change the target color in `main.py`:
  ```python
  yellow = [0, 225, 225]  # Change this BGR value to detect a different color
  ```
- Adjust HSV thresholds in `util.py` if needed.


## Author
Developed by **Harsh Panday**.

