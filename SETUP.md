# Setup Instructions for Virtual Steering Wheel

## Quick Setup (5 minutes)

### 1. Extract the Zip File
- Extract all files to a folder on your computer
- Make sure these 3 files are present:
  - `steering_wheel.py`
  - `requirements.txt`
  - `README.md`

### 2. Install Python (if not already installed)
- Download Python from https://python.org
- During installation, **check "Add Python to PATH"**
- Verify installation: Open Command Prompt and run:
  ```
  python --version
  ```
  (Should show Python 3.9 or higher)

### 3. Install Dependencies
- Open Command Prompt/Terminal
- Navigate to the project folder:
  ```
  cd path\to\virtual-steering-wheel-master
  ```
- Install required packages:
  ```
  pip install -r requirements.txt
  ```

### 4. Run the Project
- In the project folder, run:
  ```
  python steering_wheel.py
  ```
- A camera window will open
- Allow camera access if Windows asks for permission
- Press **Q** to quit

---

## Troubleshooting

### Camera not opening?
- Edit `steering_wheel.py` and change `CAMERA_INDEX` at the top:
  - Try `0` (built-in webcam)
  - Try `1` (external USB camera)
  - Try `2` if you have multiple cameras

### Python not found?
- Make sure you added Python to PATH during installation
- Or use `py` instead of `python` in commands

### Dependencies fail to install?
- Update pip first:
  ```
  python -m pip install --upgrade pip
  ```
- Then try installing again:
  ```
  pip install -r requirements.txt
  ```

---

## System Requirements
- **OS:** Windows 10/11, macOS, or Linux
- **Python:** 3.9 or higher
- **Hardware:** Webcam (built-in or USB)
- **RAM:** 4GB minimum (8GB recommended)

---

## What the Project Does
This project lets you control car games using your hands as a virtual steering wheel:
- **Both fists** = Accelerate (UP key)
- **Both hands open** = Brake (DOWN key)
- **Tilt hands left/right** = Steer

Works with any game that uses arrow keys!
