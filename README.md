👨‍💻 Internship Contribution 
During my internship, I worked on developing the Eye Tracking module for an AI-based Dyslexia and Learning Disorder Detection System. The aim of the project was to assist in the early identification of learning disabilities like dyslexia by analyzing gaze patterns, eye movements, and reading behavior in children.
This project combines computer vision, machine learning, and real-time communication to provide a low-cost, non-invasive, and accessible solution for cognitive screening.

 1. Eye Tracking Application (Standalone)
File: eyetracking.py
Captures real-time video from webcam.
Detects facial landmarks using dlib’s 68-point model.
Extracts eye contours and calculates Eye Aspect Ratio (EAR) to observe blink and focus.
Overlays real-time visual cues such as:
Eye contour shapes
Eye centers
EAR metrics

📦 Tools & Technologies:
OpenCV
dlib (Facial Landmark Predictor)
NumPy
BZ2 (for model decompression)
Python

2. Real-Time Gaze Tracking Server
File: server.py
Built using Flask and SocketIO for real-time communication with frontend clients.
Accepts base64-encoded image frames from a web or mobile frontend.
Detects eye centers and calculates normalized screen coordinates.
Emits live eye position data (left eye, right eye, average screen coordinates) back to the frontend.
Can be integrated with UI/UX interaction, reading analysis systems, or ML models.

📦 Tools & Technologies:
Flask
Flask-SocketIO
OpenCV
Dlib
Base64
Python

🚀Features
✅ Real-time eye tracking using dlib and OpenCV
✅ Frontend integration with a Flask video stream
✅ User-friendly web interface
✅ Supports multiple devices over a network


📌 Setup Instructions
1. Clone the Repository
git clone https://github.com/yourusername/eye-tracking.git cd eye-tracking
2. Install Dependencies
Install Python Packages
Make sure you have Python 3.9+ installed.
Run the following command to install required libraries: pip install flask opencv-python dlib numpy
3. Download the Pre-Trained Model
PreTrained Model
After downloading
Extract the .bz2 file using 7-Zip or any extraction tool.
Move shape_predictor_68_face_landmarks.dat to the project folder.
4. Run the Backend (Flask Server)
python app.py

📌 Expected Output:
Running on http://127.0.0.1:5000
Running on http://192.168.X.X:5000 (For local network access)
🚀 Open http://127.0.0.1:5000/video_feed in a browser to check the camera feed.

5.Run the Frontend
Simply open index.html in your browser.
✅ Click "Start Test" → Starts the user's webcam.
✅ Click "Start Tracking Now" → Switches to Flask eye-tracking feed.
✅ Click "Finish Test" → Stops tracking.

🧠 Real-World Impact
This project is designed to help:
Teachers and psychologists screen children for reading disorders early.
Institutions integrate non-intrusive assessment tools in digital classrooms.
Enable affordable and scalable AI-based solutions for cognitive health monitoring.
By building this module, I contributed to a clinical-grade application that blends AI and psychology, helping bridge the gap between education and assistive technology.
