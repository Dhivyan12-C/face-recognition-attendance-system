# 🎓 Face Recognition Attendance System

A web-based **Face Recognition Attendance Management System** built using **Python and Flask**.
The system automatically identifies registered students through their face and records attendance digitally.

It also provides separate dashboards for **teachers and students**, attendance history, permissions, activity logs, alerts, and student management.

## ✨ Features

### 👨‍🏫 Teacher Features

* Teacher login
* Student registration
* Student management
* Face registration
* Automatic face recognition
* Mark attendance using camera
* View attendance records
* Activity monitoring
* Permission management
* Holiday management
* Alerts and notifications
* Session management

### 👨‍🎓 Student Features

* Student login
* Student dashboard
* View attendance status
* View attendance history
* Submit/view permission requests
* View alerts and activities
* Profile information

### 🤖 Face Recognition

* Real-time camera-based face detection
* Registered face identification
* Automatic attendance marking
* Unknown face detection
* Face encoding storage
* Duplicate attendance prevention

### 📊 Attendance Management

* Automatic attendance recording
* Daily attendance tracking
* Student-wise attendance
* Attendance history
* Activity logs
* Digital JSON-based data storage

## 🛠️ Technologies Used

| Technology       | Purpose                     |
| ---------------- | --------------------------- |
| Python           | Backend programming         |
| Flask            | Web framework               |
| OpenCV           | Camera and image processing |
| Face Recognition | Face identification         |
| HTML             | Web page structure          |
| CSS              | User interface styling      |
| JavaScript       | Frontend interactions       |
| JSON             | Data storage                |
| Pickle           | Face encoding storage       |

## 📁 Project Structure

```text
face_attendanc/
│
├── app.py
│
├── data/
│   ├── activity_log.json
│   ├── alerts.json
│   ├── attendance.json
│   ├── credentials.json
│   ├── holidays.json
│   ├── permission.json
│   ├── permissions.json
│   ├── session_state.json
│   ├── students.json
│   ├── encodings.pkl
│   │
│   ├── faces/
│   │   └── registered student images
│   │
│   └── unknown_faces/
│
├── known_faces/
│
├── static/
│   ├── css
│   ├── images
│   ├── jss
│   └── mobile.css
│
├── templates/
│   ├── activity.html
│   ├── attendance.html
│   ├── index.html
│   ├── login.html
│   ├── menu.html
│   ├── register.html
│   ├── student.html
│   ├── students.html
│   ├── student_dashboard.html
│   ├── student_login.html
│   ├── teacher_login.html
│   └── view.html
│
└── .vscode/
```

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/face-recognition-attendance.git
```

```bash
cd face-recognition-attendance
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install flask opencv-python face-recognition numpy
```

If the project contains a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

## ▶️ Running the Application

Run:

```bash
python app.py
```

The Flask server will start locally.

Open your browser and visit:

```text
http://127.0.0.1:5000
```

## 🔄 System Workflow

```text
Student Registration
        ↓
Capture / Upload Face
        ↓
Generate Face Encoding
        ↓
Store Student Information
        ↓
Camera Starts
        ↓
Detect Face
        ↓
Compare With Registered Faces
        ↓
Student Identified
        ↓
Attendance Automatically Marked
        ↓
Attendance Stored
        ↓
Teacher / Student Dashboard
```

## 🧠 How Face Recognition Works

1. Student registers with their details.
2. The student's face image is captured.
3. The system generates a numerical **face encoding**.
4. The encoding is stored for future comparison.
5. During attendance, the camera captures the student's face.
6. The system compares the detected face with registered encodings.
7. If a match is found, the student's identity is confirmed.
8. Attendance is recorded automatically.
9. Unknown faces can be stored separately for monitoring.

## 🔐 User Roles

### Teacher

```text
Login
  ↓
Teacher Dashboard
  ↓
Manage Students
  ↓
Face Registration
  ↓
Take Attendance
  ↓
View Attendance
  ↓
Manage Permissions / Activities
```

### Student

```text
Login
  ↓
Student Dashboard
  ↓
View Attendance
  ↓
View History
  ↓
Permission / Alerts
```

## 💾 Data Storage

This project uses **JSON files** for storing application data instead of a traditional SQL database.

Examples:

* `students.json` → Student information
* `attendance.json` → Attendance records
* `credentials.json` → Login credentials
* `permissions.json` → Permission records
* `alerts.json` → Alerts
* `activity_log.json` → Activity history
* `encodings.pkl` → Face recognition encodings

## 📱 Responsive Interface

The application includes responsive styling so that the system can be accessed from different screen sizes.

```text
Desktop
   ↓
Web Application
   ↓
Responsive UI
   ↓
Mobile / Tablet Support
```

## 🔒 Security Considerations

* Separate teacher and student login
* Registered-face based identification
* Unknown face detection
* Session management
* Local data storage
* Duplicate attendance prevention

> **Note:** This project is intended primarily for educational and college project purposes. For production deployment, authentication, password storage, database security, face-data protection, HTTPS, and privacy controls should be strengthened.

## 🚀 Future Enhancements

* MySQL / PostgreSQL database integration
* Cloud deployment
* Email notifications
* WhatsApp notifications
* Advanced anti-spoofing / liveness detection
* Attendance reports in PDF/Excel
* Admin role
* Multiple camera support
* Improved authentication security
* Analytics dashboard
* Automatic monthly attendance reports

## 🎯 Project Objective

The main objective of this project is to develop an automated attendance system that uses **facial recognition technology** to identify students and record attendance, reducing manual work and improving the speed and convenience of attendance management.

## 👨‍💻 Project

**Face Recognition Attendance System**

Built with ❤️ using **Python, Flask, OpenCV and Face Recognition**.
