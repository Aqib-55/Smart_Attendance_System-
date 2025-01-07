# Smart Attendance System

## Overview
The Smart Attendance System is a Python-based project that uses face recognition technology to automate the process of marking attendance. This system detects and recognizes faces using a webcam and records attendance directly into an Excel file with timestamps.

## Features
- **Real-time Face Detection and Recognition**
- **Automatic Attendance Marking in Excel**
- **Duplicate Entry Prevention**
- **Simple Dataset Management**
- **Face Detection Before Attendance Process Begins**

## Project Structure
```
SMART_ATTENDANCE/
│
├── data_set/                            # Folder to store student images
│   ├── Aqib Raza.jpg
│   ├── Shah Rukh Khan.jpg
│   └── Emraan Hashmi.jpg
│
├── Attendance_sheet/                    # Folder for attendance Excel sheet
│   └── attendance.xlsx
│
└── source_code.py                       # Main source code for the project
```

## Requirements
- Python 3.x
- OpenCV
- face_recognition
- numpy
- openpyxl

Install the required dependencies using the following command:
```
pip install opencv-python face_recognition numpy openpyxl
```

## How to Run
1. Ensure the student dataset is placed inside `D:\SMART_ATTENDANCE\data_set`.
2. Run the project by executing the following command:
```
python source_code.py
```
3. The webcam will activate and wait until a face is detected. Once detected, the system will begin recognizing and marking attendance.
4. Press 'q' to quit the application.

## How it Works
1. The system loads known faces from the `data_set` folder.
2. It uses a webcam to capture real-time video.
3. Once a face is detected, the system matches it with the dataset and logs the entry into `attendance.xlsx` under the `Attendance_sheet` directory.
4. Duplicate entries for the same day are ignored.

## Notes
- Ensure that the Excel file is closed during attendance marking to avoid file write errors.
- Add more students by placing labeled images in the `data_set` folder.
- For better recognition, ensure that the images in the dataset are clear and of high quality.

## Contribution
Feel free to contribute by improving the recognition accuracy or adding new features. Fork the repository and create pull requests for your enhancements.


