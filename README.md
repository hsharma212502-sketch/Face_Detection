📖 Overview
Face Detection is a real-time computer vision project built in Python using OpenCV and Haar Cascade Classifiers. It taps into your live webcam feed and detects human faces frame by frame — drawing precise bounding boxes around every face it finds, in real time, with zero cloud dependency.
No APIs. No internet. No black boxes. Just raw computer vision running locally on your machine.

✨ Features

🎥 Live Webcam Detection — Processes your webcam feed in real time, frame by frame, with no lag
🧠 Haar Cascade Classifier — Uses OpenCV's pre-trained haarcascade_frontalface_default.xml for fast and accurate face localization
🟩 Bounding Box Rendering — Draws precise green rectangles around every detected face instantly
👥 Multi-Face Support — Detects and marks multiple faces simultaneously in a single frame
⚡ Lightweight & Fast — Runs entirely on CPU with no GPU or cloud infrastructure required
🔒 100% Offline — All processing happens locally — no data leaves your machine
🧼 Zero-Fluff Codebase — Clean, readable Python with minimal dependencies
🛑 Graceful Exit — Press Q at any time to cleanly terminate the webcam session


🛠️ Tech Stack
ToolPurposePython 3.7+Core languageOpenCV (cv2)Video capture, image processing, renderingHaar CascadesPre-trained face detection classifier

⚙️ Installation & Setup
Prerequisites
Make sure Python is installed:
bashpython --version  # Requires Python 3.7+
Clone the Repository
bashgit clone https://github.com/yourusername/face-detection-opencv.git
cd face-detection-opencv
Install Dependencies
bashpip install opencv-python<br>

The Haar Cascade XML file ships with OpenCV — no additional downloads needed.<br>
<br>

▶️ How to Run<br>
Launch the detector with a single command:<br>
bashpython face_detection.py<br>
Your webcam will activate instantly. The system will begin detecting faces in real time and drawing bounding boxes around each one found.<br>
Controls:<br>
KeyActionQQuit and close the webcam window<br>
Example Output:<br>
[INFO] Starting webcam feed...<br>
[INFO] Face detection active. Press 'Q' to quit.<br>
[INFO] Faces detected in frame: 2<br>
[INFO] Faces detected in frame: 1<br>
[INFO] Session ended by user.<br>

📁 Project Structure<br>
face-detection-opencv/<br>
│
├── face_detection.py                    # Main detection script<br>
├── haarcascade_frontalface_default.xml  # Pre-trained Haar Cascade model<br>
└── README.md                            # Project documentation<br>

🧠 How It Works<br>

Capture — OpenCV opens the default webcam and reads a continuous stream of frames<br>
Preprocess — Each frame is converted to grayscale to reduce computational load<br>
Detect — The Haar Cascade classifier scans the grayscale frame for face-like patterns<br>
Render — Bounding boxes are drawn around every detected face on the original color frame<br>
Display — The annotated frame is displayed in real time in an OpenCV window<br>
Loop — The process repeats for every frame until the user quits<br>


🤝 Contributing<br>
Contributions, issues, and feature requests are welcome. Fork the repo, make your changes, and submit a pull request.<br>
