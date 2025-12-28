✋ Hand Gesture Based Volume & Brightness Control (macOS)

Control your MacBook’s system volume and screen brightness using hand gestures captured through the built-in webcam.

Left Hand → Volume control

Right Hand → Brightness control

Gesture → Distance between thumb and index finger

This project uses Computer Vision and MediaPipe hand tracking and requires no external hardware.
<img width="922" height="332" alt="image" src="https://github.com/user-attachments/assets/e905cab2-5f22-4752-b211-4696e5dfbfea" />


📌 Project Highlights

Real-time hand tracking using webcam
Accurate Left / Right hand identification
Smooth thumb–index distance mapping
Native macOS volume & brightness control
Works on Intel and Apple Silicon Macs

🧠 How It Works

Webcam captures live video
MediaPipe detects hand landmarks (21 points per hand)
Distance between thumb tip (4) and index tip (8) is calculated
Distance is mapped to a 0–100 scale

Based on hand:
Left → System Volume
Right → Screen Brightness

🧰 Tech Stack
Python 3.9+
OpenCV
MediaPipe
NumPy
macOS AppleScript
Screen Brightness Control

📁 Project Structure

gesture-control/
│
├── gesture_control.py
├── README.md
└── requirements.txt

⚙️ Installation & Setup (Step-by-Step)
1️⃣ Check Python Version
python3 --version


Python 3.9 or higher required.

2️⃣ Create Virtual Environment (Recommended)
python3 -m venv venv
source venv/bin/activate

3️⃣ Install Dependencies
pip install opencv-python mediapipe numpy screen-brightness-control

4️⃣ macOS Permissions (CRITICAL)

Go to System Settings → Privacy & Security

✔ Camera → Allow Terminal / Python
✔ Accessibility → Allow Terminal / Python

Without Accessibility permission, volume control will NOT work.

▶️ Running the Program
python3 gesture_control.py


Press Q to exit.

✋ Gesture Usage Guide
Hand	Gesture	Action
Left	Thumb–Index apart	Volume ↑
Left	Thumb–Index closer	Volume ↓
Right	Thumb–Index apart	Brightness ↑
Right	Thumb–Index closer	Brightness ↓
