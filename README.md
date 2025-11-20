# Traffic Violation Detection

This project automatically detects traffic rule violations such as signal jumping, wrong lane driving, illegal parking, and also extracts vehicle number plates using OCR. It stores violation details using SQLite for easy tracking and challan generation.

## Features
- Signal violation detection
- Wrong lane detection
- Parking violation detection
- Vehicle number plate recognition (OCR)
- Violation data storage using SQLite

## Technologies Used
- Python
- OpenCV
- YOLO (for object detection)
- pytesseract (for OCR)
- SQLite (for storing challan data)

## How to Use
1. Download or clone this repository.
2. Install the required libraries
3. Install Tesseract OCR
  Download and install from:
  https://github.com/tesseract-ocr/tesseract
  Add the installed Tesseract path to your system’s environment variables
  For example, on Windows:
  C:\Program Files\Tesseract-OCR
4. Run the Main Script
python main.py

🗃️ SQLite Database Info
The project stores violation data (like vehicle number, type of violation, timestamp) in an SQLite database file, violations.db.

Sample Table Structure: 
CREATE TABLE violations (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    vehicle_number TEXT,
    violation_type TEXT,
    timestamp TEXT,
    location TEXT
);

📌 Future Improvements
1. Real-time video stream detection
2. Automated challan generation with PDFs
3. Integration with government APIs or SMS alerts

👩‍💻 Author

Neha Kataria
