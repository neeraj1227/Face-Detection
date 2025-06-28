🧠 Face Detection Project
Welcome to the Face Detection project! This simple project demonstrates how to detect human faces in images or real-time video using Python and OpenCV.

📌 Features
Detects faces in static images

Real-time face detection using webcam

Highlights detected faces with bounding boxes

🛠️ Requirements
Python 3.x

OpenCV (opencv-python)

Install Dependencies

pip install opencv-python


🚀 Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/face-detection.git
cd face-detection

🧪 Example Code
face-detection.py
python
Copy
Edit
import cv2

# Load the cascade
face_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')

# Read the input image
img = cv2.imread('')
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# Detect faces
faces = face_cascade.detectMultiScale(gray, 1.1,5)

# Draw rectangles around faces
for (x, y, w, h) in face:
    cv2.rectangle(img, (x, y), (x+w, y+h), (255, 0, 0), 2)

# Display result
cv2.imshow('Detected Faces', img)
cv2.waitKey()
break


📷 Example Output
When you run the script, the program will show the input image with rectangles drawn around detected faces.


📚 Resources
OpenCV Python Docs

Face Detection with Haar Cascades


🙌 Contribution
Feel free to fork, contribute, or ask questions!


📝 License
This project is licensed under the MIT License.

