# 🖐️ Hand Tracking Canvas 🎨 (HTC Project)

Create a virtual canvas where you can draw in the air using just your **fingers and webcam** — no mouse or touch required!

Built with 🐍 Python, using 🔍 OpenCV and 🤚 MediaPipe for real-time hand tracking and drawing.  
Ideal for beginners in computer vision, gesture control, or anyone who wants to explore a fun mini-project.

---

## 📌 Project Features

✅ Real-time hand tracking using your webcam  
✅ Draw on the screen using index finger  
✅ Switch between pen and eraser with gestures  
✅ Easily customizable brush size, color, gestures  
✅ Simple Python code — beginner-friendly and clean

---

## 🧠 Technologies Used

| Tool        | Description                            |
|-------------|----------------------------------------|
| Python 3.11.9| Programming language                  |
| OpenCV      | Video capture and image processing     |
| MediaPipe   | Real-time hand landmark detection      |
| NumPy       | Array operations for canvas overlays   |

---

## 📁 Project Files Overview

| File Name           | Description                                           |
|---------------------|-------------------------------------------------------|
| `HandTracking.py`   | Detects hands and finger positions using MediaPipe    |
| `Virtualcanvas.py`  | Main app file — drawing canvas logic and gesture flow |
| `t.py`              | Optional test/helper file                             |
| `.gitignore`        | Ignores cache and unnecessary files                   |
| `__pycache__/`      | Python-generated cache folder (auto ignored)          |

---

## 🖥️ Requirements & Setup

### ✅ 1. Install Python 3.11.9  
Download and install from the official site:  
🔗 [https://www.python.org/downloads/release/python-3119/](https://www.python.org/downloads/release/python-3119/)

### ✅ 2. Install Required Packages  
Open your terminal or VS Code terminal and run:
```bash
pip install opencv-python mediapipe numpy

```
▶️ How to Run the Project

💻 Using VS Code (or any terminal):

1.Open your terminal inside the project folder.

2.Run the main file:

```bash
  python Virtualcanvas.py
 ```
3.Your webcam will open, and you’ll see your video feed with a canvas.

4.Move your hand in front of the webcam to start drawing!

✋ How to Control the Canvas (Gestures)

| Action           | What to Do                                   |
| ---------------- | -------------------------------------------- |
| ✏️ Start Drawing | Raise **only index finger**                  |
| 🧽 Erase         | Raise **two fingers** (index + middle) select eraser and erase using index finger |
| 🟥 Change Colors | Raise **two fingers** (index + middle) select color  |
| ❌ Exit the App   | Press **`ctrl+c`** key in terrminal |

All gestures are detected using real-time hand landmarks — no buttons required!

🧠 How the Project Works

1.OpenCV captures the webcam feed frame-by-frame.

2.MediaPipe detects and tracks 21 landmarks on your hand.

3.The index finger tip is used as a drawing pointer.

4.Drawing happens when only index finger is up (gesture logic).

5.The canvas overlays are blended with the webcam video.

🧰 How to Customize or Modify

| Want to Change This?           | How to Do It                                       |
| ------------------------------ | -------------------------------------------------- |
| 🎨 Add more colors             | Edit the color palette in `Virtualcanvas.py`       |
| ✏️ Increase brush size         | Adjust brush thickness variable in code            |
| 🖐️ Use new gestures           | Modify finger count logic in `HandTracking.py`     |
| 🎞️ Save your drawing as image | Add `cv2.imwrite()` at the end of the drawing loop |
| 📷 Use second webcam           | Change `cv2.VideoCapture(0)` to `(1)`              |

🧯 Troubleshooting
| Problem                             | Solution                                                |
| ----------------------------------- | ------------------------------------------------------- |
| ❌ ModuleNotFoundError for mediapipe | Run: `pip install mediapipe`                            |
| 📷 Webcam not opening               | Ensure no other app is using the webcam                 |
| 🛑 Program exits instantly          | Make sure `Virtualcanvas.py` is the file you're running |
| 🤚 Drawing doesn’t start            | Only keep index finger up, steady in front of cam       |

🧪 Example Use Case

1.Build an AI Drawing App

2.Teach computer vision concepts

3.Fun hackathon or college project

4.Replace mouse-based painting apps

5.Can be used in touchless interaction systems 


👨‍💻 Author

Shashidhar

🔗 GitHub: @mail2shashi11


⭐ Support & Sharing

If this project helped you, please consider:

🌟 Starring the repo

🍴 Forking and modifying it

📢 Sharing it with others

💬 Suggesting improvements

Thank you for checking out the Hand Tracking Canvas Project!

