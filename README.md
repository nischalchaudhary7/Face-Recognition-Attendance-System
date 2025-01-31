An AI-powered attendance system using Python, OpenCV, and Tkinter to automate student attendance tracking through real-time face recognition. It integrates MySQL for efficient data management and supports CSV import/export for seamless record handling.

Face Recognition Attendance System 🎓📷
An AI-powered attendance system using Python, OpenCV, and Tkinter to automate student attendance tracking through real-time face recognition. It integrates MySQL for efficient data management and supports CSV import/export for seamless record handling.

 1.Features
 Real-time Face Recognition with 77% accuracy
 Automated Attendance Marking with CSV & MySQL storage
 Student Registration & Management
 User-Friendly GUI built with Tkinter
 Modular System with separate panels for Training, Attendance, and Help Support

2.Tech Stack
Python, OpenCV, Tkinter
MySQL (Database), CSV (Data Handling)
NumPy, Pandas, PIL

3. Project Structure
 📂 Face-Recognition-Attendance-System
  📂 dataset        # Stores captured images
  📂 Images_GUI     # GUI images
  📂 data_img       # Processed images
  📜 main.py        # Launches the application
  📜 face_recognition.py  # Face detection & recognition logic
  📜 train.py       # Trains the model
  📜 student.py     # Manages student data
  📜 attendance.py  # Attendance tracking
  📜 requirements.txt  # Dependencies
  📜 README.md      # Documentation

4.How It Works?
 Register Students – Capture face images & store data
 Train the Model – Uses LBPH Face Recognizer
 Recognize Faces – Matches live faces with stored data
 Mark Attendance – Records attendance in MySQL & CSV
 View & Export Data – Retrieve attendance reports
