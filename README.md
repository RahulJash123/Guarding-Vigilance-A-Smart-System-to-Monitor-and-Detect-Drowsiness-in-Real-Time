# DrowZense – Driver Drowsiness Detection System

DrowZense is a desktop application that detects driver drowsiness in real-time using a webcam. It uses facial landmarks to monitor eye closure, yawning, and head tilt, then gives alerts if signs of fatigue are detected.

---

## 🚀 Features

- Detects prolonged eye closure (blinks)
- Detects yawning and head tilting
- Real-time video analysis using webcam
- Voice alerts using text-to-speech (pyttsx3)
- Custom GUI built using CustomTkinter
- Statistics panel for recent alerts
- Gemini AI integration to summarize alert data

---

## 🧰 Technologies Used

- Python (OpenCV, MediaPipe, pyttsx3, Pandas, CustomTkinter)
- Electron.js (Node.js + Chromium GUI)
- HTML, CSS, JavaScript
- Google Gemini API (for statistical analysis)

---

### Python Dependencies

drowzense/
│
├── index.html           # Electron frontend
├── main.js              # Electron app entry
├── renderer.js          # Executes Python script from Electron
├── script.js            # UI animations & scroll
├── style.css            # App styling
│
├── python/
│   ├── 1.py             # Main detection system (CustomTkinter GUI)
│   ├── 2.py             # Gemini-based stats summary
│   └── drowsiness_data.csv # Output data file
│
├── package.json         # Node app config
└── README.md            # You're here!

---

### Output

- Realtime webcam feed with status panel
- Logs signs like:
  - Prolonged blink
  - Yawning
- Head tilt
- Alerts appear based on severity
- Summary generated via Gemini (based on CSV data)

