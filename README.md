A modern hospital management system that replaces traditional hospital cards with QR codes for patient identification and tracking.

## Features

- Patient Registration with QR Code Generation
- Appointment Booking System
- Payment Integration (Telebirr and Chapa)
- Admin Dashboard with Analytics
- Medical Records Management
- Doctor Management

## Installation

1. Create a virtual environment:
```bash
# Create a new virtual environment
python3 -m venv venv

# Activate the virtual environment
# On Linux/macOS:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

# Verify installation:
The following packages should be installed:
- Flask==3.0.2
- qrcode[pil]==7.4.2
- plotly==5.19.0
- Werkzeug==3.0.1
- pillow==10.2.0

3. Initialize the database:
```bash
python app.py
```

4. Access the application:
Visit `http://127.0.0.1:5000` in your web browser

## Project Structure

```
hospital_cardless_system/
├── app.py                 # Main application file
├── database.db           # SQLite database
├── requirements.txt      # Project dependencies
├── static/              # Static files
│   └── qr_codes/       # Generated QR codes
└── templates/          # HTML templates
```

## Security Notes

- All passwords are hashed before storage
- Admin routes are protected with authentication
- QR codes are securely generated and stored
