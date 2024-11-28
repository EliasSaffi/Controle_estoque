# Inventory Control System

A multi-language inventory management system built with Python and Flet, featuring QR code integration and real-time stock tracking.

## Features

- 🌐 Multi-language support (English, Portuguese, Spanish)
- 🔐 User authentication and role-based access control
- 📦 Product management with QR code generation
- 📊 Stock movement tracking (entries/exits)
- 👥 Supplier management
- 🎨 Light/Dark theme toggle
- 📱 Responsive design
- 📷 QR code scanning for quick stock operations

## Prerequisites

- Python 3.8+
- MySQL Server (XAMPP recommended)
- Webcam (for QR code scanning)

## Installation

1. Clone the repository:

bash
git clone https://github.com/yourusername/inventory-control-system.git
cd inventory-control-system

2. Create a virtual environment and activate it:

bash
python -m venv venv
source venv/bin/activate # Linux/Mac
venv\Scripts\activate # Windows

3. Install required packages:

bash
pip install -r requirements.txt


4. Set up the database:
   - Start MySQL server (via XAMPP or other method)
   - Import `database.sql` into your MySQL server

## Required Packages

txt
flet>=0.9.0
mysql-connector-python>=8.0.0
qrcode>=7.3
opencv-python>=4.5.0
numpy>=1.19.0
Pillow>=8.0.0

## Configuration

1. Database configuration (in `main.py`):

python
connection = mysql.connector.connect(
host="localhost",
user="root",
password="", # Update if you have set a password
database="inventory_system"
)

## Usage

1. Start the application:

bash
python main.py

2. Default admin credentials:
   - Username: `admin`
   - Password: `admin123`

## Features Overview

### User Management
- Create/Edit/Delete users
- Assign roles (Admin/User)
- Role-based access control

### Product Management
- Add/Edit/Delete products
- Generate QR codes for products
- Track stock levels
- Scan QR codes for quick operations

### Stock Operations
- Record stock entries
- Record stock exits
- View movement history
- QR code scanning for quick operations

### Additional Features
- Multi-language support
- Theme switching
- Help documentation
- Movement history tracking

## Security Features

- User authentication
- Role-based access control
- Admin-only sections
- Login required for sensitive operations

## Acknowledgments

- [Flet](https://flet.dev/) for the UI framework
- [OpenCV](https://opencv.org/) for QR code scanning
- [QRCode](https://pypi.org/project/qrcode/) for QR code generation

## Screenshots

[Someday...]