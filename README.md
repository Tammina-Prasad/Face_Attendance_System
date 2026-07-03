# Face Attendance System

A Python-based Face Attendance System that automatically recognizes registered users through a webcam and records attendance with date and time. This eliminates manual attendance, reduces errors, and prevents proxy attendance.

---

## Features

- Register new users using a webcam
- Automatic face recognition in real time
- Attendance stored in an Excel file with timestamps
- User-friendly desktop GUI
- SQLite database for user management
- Optional Flask API support

---

## Project Structure

```
Face-Attendance-System/
│── add_person.py            # Register new users
│── train_model.py           # Train face encodings
│── recognition_helper.py    # Real-time face recognition
│── update_excel.py          # Create/update attendance sheet
│── gui.py                   # Desktop application
│── app.py                   # Optional Flask API
│── init_db.py               # Initialize SQLite database
│── dataset/                 # Captured face images
│── attendance.xlsx          # Attendance records
│── requirements.txt
│── README.md
```

---

## Tech Stack

- Python
- OpenCV
- face_recognition (dlib)
- Pandas
- OpenPyXL
- CustomTkinter
- SQLite
- Flask

---

## Installation

### Clone the repository

```bash
git clone https://github.com/<Tammina-Prasad >/Face-Attendance-System.git
cd Face-Attendance-System
```

### Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python -m venv venv
source venv/bin/activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## Usage

### 1. Initialize the database

```bash
python init_db.py
```

### 2. Create the attendance sheet

```bash
python update_excel.py
```

### 3. Register a new person

```bash
python add_person.py
```

### 4. Train the recognition model

```bash
python train_model.py
```

### 5. Start the application

```bash
python gui.py
```

---

## How It Works

1. Register a user by capturing face images through the webcam.
2. Train the model to generate face encodings.
3. Launch the application.
4. The webcam detects and recognizes registered users.
5. Attendance is automatically recorded in an Excel sheet with the current date and time.

---

## Future Improvements

- Multiple camera support
- Face mask detection
- Email attendance reports
- Cloud database integration
- Web dashboard
- Anti-spoofing (photo/video attack detection)

---

## Author

**Tammina Prasad**