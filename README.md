<h1>Face Recognition System</h1>

A Python-based Face Recognition System that can recognize known faces from a dataset and also perform real-time recognition via webcam using the face_recognition and OpenCV libraries.

<h2><u>Features</u></h2>

*Load and encode known faces from a folder

*Detect and recognize faces in unknown images

*Perform real-time face recognition through webcam

*Draw bounding boxes and labels around detected faces

*Handles unknown faces gracefully

<h2><u>Tech Stack</u></h2>

~Python 3

~face_recognition

~OpenCV (cv2)

~NumPy

~Pillow (PIL)

<h2><u><b>Project Structure</b></u></h2>  

```bash
face_recognition_project/
├── known_faces/        # Store known face images (e.g., "Alice.jpg")
├── unknown_faces/      # Store test/unknown images for recognition
├── recognize_images.py # Script to recognize faces in images
├── recognize_webcam.py # Script for real-time webcam recognition
└── README.md           # Project documentation
``` 

<h2><u>Installation</u></h2>

```bash
#Clone the repository

git clone https://github.com/pawni-purity/face-recognition-system.git
cd face_recognition_project

#Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

#Install dependencies
pip install face_recognition opencv-python pillow numpy
```

<h2><u>Usage</u></h2>
1.Recognize Faces in Images

Place known faces in known_faces/ and test images in unknown_faces/.

Run:
python recognize_images.py

2.Real-time Recognition with Webcam

Run:
python recognize_webcam.py

Press q to quit.

<h2><u>Notes</u></h2>

#Ensure images in known_faces/ contain clear, single faces.

#Filenames are used as labels (e.g., Alice.jpg → Alice).

#Performance may drop with poor lighting or blurry images.

<h2><u>Future Improvements</u></h2>

Add a GUI for uploading and testing images

Store encodings in a database for faster lookups

Improve accuracy with deep learning-based models
