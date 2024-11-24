# Face Recognition System
This is a simple face recognition application built using Python. It leverages the face_recognition library to identify and recognize faces from a live webcam feed. The application can recognize faces that are pre-encoded and stored in a specified directory.

## Features
- Real-time face detection and recognition using a webcam.
- Displays the names of recognized individuals along with confidence levels.
- Handles unknown faces gracefully.
- Supports multiple known faces.

## Requirements
To run this application, you'll need the following:

- Python 3.x
- OpenCV
- NumPy
- face_recognition
- A webcam

You can install the required libraries using pip:

```bash
pip install -r requirements.txt
```

## Setup
1. Clone the Repository:

```bash
git clone https://github.com/amt278/face_recognition.git
cd face_recognition
```

2. Prepare Known Faces:
   - Add images of the individuals you want to recognize in the faces directory. The filenames will be used as the names for recognition (e.g., john_doe.jpg will be recognized as "john_doe").

3. Run the Application:

```bash
python face_recognition.py
```

4. Usage:
   - The application will open a window displaying the webcam feed.
   - It will attempt to recognize faces in the feed and display the names along with confidence percentages.
   - Press 'q' to quit the application.

## Code Overview
- face_confidence: A function that computes the confidence level of a face match based on the distance between face encodings.
- FaceRecognition Class:
  - Initializes by encoding known faces from the faces directory.
  - Handles the webcam feed and performs face recognition in real-time.
