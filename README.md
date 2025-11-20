🚦 AI-Based Traffic Violation Detection System

This project is an intelligent traffic monitoring system that automatically detects traffic violations such as signal jumping, wrong-lane driving, and illegal parking using computer vision. It also extracts vehicle number plates using OCR and stores all violation records in an SQLite database for easy tracking and challan generation.

🔍 Key Features

- 🚨 Traffic signal violation detection

- 🛣️ Wrong-lane driving detection

- 🅿️ Illegal parking detection

- 🔢 Automatic number plate recognition using OCR

- 💾 SQLite database integration for violation and challan records

- 📊 Easy-to-view logs via GUI (PyQt5)

- 🛠️ Technologies Used

Python 3

OpenCV – for image & video processing

YOLO – for vehicle and object detection

pytesseract – for number plate OCR

PyQt5 – for graphical user interface

SQLite – for database management

imutils, NumPy, etc. – for image utilities

📦 Setting Up Virtual Environment

Follow these steps to create and activate a virtual environment:

On Windows
- python -m venv traffic
- traffic\Scripts\activate

On Linux / Mac
- python3 -m venv traffic
- traffic/bin/activate


Once activated, your terminal will show (traffic) at the beginning.

📥 Installing Required Libraries

After activating your environment, install all dependencies from requirements.txt:

- pip install -r requirements.txt

🖥 Installing Tesseract OCR

Since the project uses OCR for number plate recognition, you must install Tesseract.

Steps for Windows:

Download from:
👉 https://github.com/tesseract-ocr/tesseract

Install it.

Add this path to your System Environment Variables:

C:\Program Files\Tesseract-OCR


Verify installation:

tesseract --version

▶ How to Run the Project

After installing dependencies and OCR:

python main.py


This will launch the GUI application and start violation detection.

🗄️ Database Information

The system stores all violation details in an SQLite database:

Database File: violations.db

Sample table structure:
CREATE TABLE violations (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    vehicle_number TEXT,
    violation_type TEXT,
    timestamp TEXT,
    location TEXT
);

🚀 Future Enhancements

🎥 Real-time live camera streaming

🧾 Automated E-Challan PDF generation

📲 SMS / Email alerts for vehicle owners

🌐 Integration with RTO or Government APIs

🤖 Improved AI models for better accuracy

👤 Author

Aakash Meena
📧 Email: aakashmeena421@gmail.com