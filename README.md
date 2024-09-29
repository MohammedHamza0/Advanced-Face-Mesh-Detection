# Advanced Face Mesh Detection

This project implements **Advanced Face Mesh Detection** with real-time head pose estimation and eye closure monitoring, using **Mediapipe**, **OpenCV**, and **Python**. The system is capable of detecting head movements (looking left, right, up, down, or facing forward) and detecting if the eyes are closed. This project is useful for both **driver monitoring systems** and **student attention tracking**.

## Features
- **Real-time Face Mesh Detection**: Detects 3D facial landmarks using Mediapipe's Face Mesh solution.
- **Head Pose Estimation**: Calculates pitch, yaw, and roll angles to estimate the direction of a person's head.
- **Eye Aspect Ratio (EAR)**: Measures eye openness to detect if eyes are closed.
- **Warnings**: Issues alerts when the head is not facing forward or if eyes are closed.
- **Live Video Feed**: Processes input directly from the webcam and overlays the results on the video stream.
- **Frame Rate (FPS)**: Displays real-time FPS to ensure smooth processing.

## Applications
1. **Driver Monitoring System**
   - Detects if a driver is distracted (e.g., looking away) or drowsy (eyes closed).
   - Issues warnings like "Please face forward" and "Eyes are closed."

2. **Student Monitoring System**
   - Helps track student focus in online or in-person learning.
   - Detects when a student is not paying attention or falling asleep.

## Installation

### Prerequisites
- Python 3.x
- OpenCV
- Mediapipe
- Numpy
- Scipy

### Installation Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/MohammedHamza0/advanced_face_mesh_detection.git
   cd advanced_face_mesh_detection
   ```



3. Open the `advanced_face_mesh_detection.ipynb` file in Jupyter Notebook or any compatible environment:
   ```bash
   jupyter notebook advanced_face_mesh_detection.ipynb
   ```

## Usage
1. Run the notebook, and your webcam will automatically activate.
2. The system will detect your facial landmarks and monitor your head pose and eye aspect ratio (EAR).
3. Real-time results will be displayed on the video feed, including head orientation (left, right, up, down) and whether your eyes are closed.
4. Warnings will appear on the video feed when needed.

## Key Sections in the Notebook
- **Face Mesh Detection**: Using Mediapipe to capture 468 3D facial landmarks.
- **Head Pose Estimation**: Using 6 specific landmarks to calculate head rotation angles (pitch, yaw, roll).
- **Eye Aspect Ratio (EAR)**: Monitoring eye openness to detect blinking or prolonged closure.
- **Warnings**: Real-time display of warnings based on head and eye movements.

## Example
The system will print and display information such as:

```
Right EAR: 0.25, Left EAR: 0.26, Avg EAR: 0.255
Head Status: Looking Left
Warning: Please face forward!
```


## Future Enhancements
- **Fatigue Detection**: Enhance eye closure monitoring to detect drowsiness more accurately.
- **Emotion Recognition**: Integrate emotion detection using the facial landmarks.
- **Multi-person Detection**: Expand to detect and monitor multiple people in the frame simultaneously.

## Contributing
Pull requests are welcome! If you have suggestions for improvements, feel free to submit them or open an issue.

