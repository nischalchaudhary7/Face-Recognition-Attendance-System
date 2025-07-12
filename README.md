Face Recognition Attendance System

This is a complete Python-based Face Recognition Attendance System that helps automate attendance using facial recognition. The system captures student photos, trains a face recognition model, and marks attendance in real time through your webcam. It also includes admin login, a GUI, database connection, and support links.

 What This Project Can Do
 Admin login and user authentication

 Student registration with name, ID, and photo capture

 Train a face recognition model using saved images

 Detect and recognize student faces live from a webcam

 Record attendance with date and time

 Store data in a MySQL database (configured on port 3307)

 Includes a Developer Info screen


🛠️ Tools & Technologies Used
Technology	Purpose
Python 3.8.5	Main programming language
OpenCV	Face detection and recognition
MySQL	Stores student and attendance data
Tkinter	Used for building the GUI
Pillow (PIL)	Handles image files in the GUI
CSV	Saves attendance records locally

📂 Files & Folder Overview
pgsql
Copy
Edit
Face-Recognition-Attendance-System/
├── main.py                    → Main interface to launch everything
├── login.py                   → Login screen for admin
├── register.py                → Register new admin users
├── student.py                 → Register students & capture images
├── train.py                   → Train the face recognition model
├── face_recognition.py        → Runs real-time face recognition
├── attendance.py              → View or manage attendance records
├── developer.py               → About the developer panel
├── helpsupport.py             → External support links (YouTube, Gmail, etc.)
├── databaseTest.py            → Test DB connection
├── haarcascade_frontalface_default.xml → Face detection XML file
├── clf.xml                    → Model file saved after training
├── attendance.csv             → Generated attendance log file
├── Images_GUI/                → Icons and images for GUI
├── data_img/                  → Folder to store student face images
└── requirements.txt           → List of Python dependencies

▶️ How to Run the Project

1. Prerequisites
Before running the system, make sure you have:

Python 3.8.5 (64-bit)

MySQL installed and running on port 3307

Any code editor like VS Code

2. Install Required Libraries
You can install the required Python packages with:

bash
pip install opencv-python
pip install numpy
pip install pillow
pip install mysql-connector-python
Or all at once:

bash
pip install -r requirements.txt
3. Set Up MySQL Database
Open MySQL and run:

sql

CREATE DATABASE face_recognition;
Tables like student and regteach will be created automatically by the code. Make sure your DB config in the Python files uses:

python

username='root', password='root', host='localhost', port=3307
You can update this in databaseTest.py, face_recognition.py, etc., if your settings are different.

4. Start the App
Simply run:

python main.py
And follow the interface to register students, train the model, and take attendance!

 Want to Show Off?
Feel free to include screenshots of your UI, student registration window, and live recognition in this section for better presentation.


How Face Recognition Works
It uses Haar Cascades for face detection and LBPH (Local Binary Patterns Histograms) for recognition.

The confidence threshold is set at 77% — attendance is only marked if confidence is better.

Duplicate entries are prevented in the same session.
