"""
Real-Time Face Verification (DeepFace + OpenCV)
=======================================================

This program performs real-time face verification using your webcam.
It compares the face from the camera with a reference image `reference.jpg`.

FEATURES
- Live webcam feed (OpenCV)
- Face verification using DeepFace
- Multi-threaded verification to keep the video smooth
- Visual feedback: MATCH / NO MATCH on the video

REQUIREMENTS
Python 3.8+

FILES
- This .py file
- reference.jpg (face image to compare)

HOW IT WORKS
1. The webcam captures frames continuously
2. Every 30 frames, a separate thread performs face verification
3. DeepFace compares the current frame with reference.jpg
4. The result is displayed on the screen

USAGE
    python face_verify.py

CONTROLS
- q → quit the program

NOTES
- Good lighting improves accuracy
- reference.jpg should contain a clear face
- On first run, DeepFace will download necessary models automatically

LICENSE
For educational and testing purposes.
"""
