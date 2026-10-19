<<<<<<< HEAD
# 🎓 Smart Attendance System Using Face Recognition

##  Project Overview

The **Smart Attendance System Using Face Recognition** is a Python-based application that automates student attendance using a webcam. It uses OpenCV for face detection and the LBPH algorithm for face recognition.

The system allows users to register students, capture their face images, train a recognition model, and mark attendance. Attendance records are stored in CSV files for easy access and management.

##  Features

* **Student Registration:** Register students using their ID and name.
* **Face Detection:** Detect faces using the Haar Cascade classifier.
* **Face Recognition:** Recognize registered students using the LBPH algorithm.
* **Image Capture:** Capture and store face images for training.
* **Model Training:** Train the recognition model using registered face images.
* **Automated Attendance:** Record recognized students' attendance using a webcam.
* **CSV Records:** Store student details and attendance records in CSV format.
* **Graphical User Interface:** Use a desktop interface built with Tkinter.
* **Live Clock and Date:** Display the current date and time in the application.

##  Technologies Used

| Technology   | Purpose                              |
| ------------ | ------------------------------------ |
| Python       | Main programming language            |
| OpenCV       | Face detection and image processing  |
| Haar Cascade | Detect faces in webcam images        |
| LBPH         | Recognize registered faces           |
| Tkinter      | Build the graphical user interface   |
| NumPy        | Handle image data as arrays          |
| Pandas       | Read and process student records     |
| CSV          | Store student details and attendance |
| Pillow (PIL) | Process images                       |

##  Requirements

* Python 3.9 or a compatible Python version
* A working webcam
* pip package manager
* Required Python libraries

## 🚀 Installation and Setup

### 1. Clone the Repository

### 2. Open the Project Folder

```bash
cd Smart-Attendance-System-Using-Face-Recognition
```

### 3. Install Required Libraries

```bash
python -m pip install opencv-contrib-python numpy pandas pillow
```

**Note:** The `opencv-contrib-python` package is required for the LBPH face recognizer.

### 4. Run the Application

```bash
python main.py
```

Ensure that `haarcascade_frontalface_default.xml` is present in the project folder before running the application.

##  Project Structure

```text
Smart-Attendance-System-Using-Face-Recognition/
│
├── Attendance/
│   └── Attendance records saved as CSV files
│
├── StudentDetails/
│   └── StudentDetails.csv
│
├── TrainingImage/
│   └── Captured student face images
│
├── TrainingImageLabel/
│   └── Trainner.yml
│
├── haarcascade_frontalface_default.xml
├── main.py
└── README.md
```

The application creates the required directories when they do not already exist. Student images, student details, and trained model files are generated as the application is used.

##  How the System Works

### Step 1: Student Registration

Enter the student's ID and name in the application.

### Step 2: Capture Face Images

Click **Take Images** to capture face images through the webcam. The images are saved in the `TrainingImage` folder.

### Step 3: Train the Recognition Model

Click **Save Profile** and complete the password prompt. The system trains the LBPH recognizer using the captured images and saves the trained model as `Trainner.yml`.

### Step 4: Take Attendance

Click **Take Attendance** to start webcam-based face recognition.

### Step 5: Save Attendance Records

The system identifies recognized students and stores attendance information in date-wise CSV files inside the `Attendance` folder.

##  Face Detection vs Face Recognition

**Haar Cascade:** Detects the location of a face in an image.

**LBPH (Local Binary Patterns Histograms):** Compares a detected face with the trained face data to predict the registered student.

Both techniques work together to support the attendance process.

## Data Storage

The project uses CSV files and local folders to store its data.

* `StudentDetails/StudentDetails.csv` — Stores student IDs, names, and serial numbers.
* `TrainingImage/` — Stores captured face images.
* `TrainingImageLabel/Trainner.yml` — Stores the trained face recognition model.
* `Attendance/` — Stores date-wise attendance records.

##  Troubleshooting

**1. Face detection is not working**

* Ensure your webcam is connected and working.
* Check that `haarcascade_frontalface_default.xml` is present in the project folder.
* Use sufficient lighting and keep your face visible to the camera.

**2. LBPH face recognizer is unavailable**
Install the required OpenCV package:

```bash
python -m pip install opencv-contrib-python
```

**3. No registered students found during training**

* Register a student first.
* Capture face images successfully.
* Check that the `TrainingImage` folder contains valid images.

**4. Webcam is not opening**

* Close other applications using the webcam.
* Check your camera permissions.
* Ensure that the correct camera is selected.

##  Future Improvements

* Prevent duplicate attendance entries.
* Add an attendance report export feature.
* Integrate a database such as MySQL or SQL Server.
* Add administrator authentication and improved password security.
* Develop a web-based attendance dashboard.
* Improve recognition performance under different lighting conditions.

##  Privacy and Security

This project processes face images and student attendance records. Use it with appropriate permission and protect all personal information.

Do not upload private student face images, real attendance records, or password files to a public repository.

##  Learning Outcomes

Through this project, I gained practical experience with:

* Python application development
* OpenCV and image processing
* Face detection and recognition
* Haar Cascade and LBPH
* Tkinter GUI development
* CSV-based data management
* Webcam integration

##  Author

**Shubham Singh**
=======

