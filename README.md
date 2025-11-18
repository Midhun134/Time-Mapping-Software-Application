## Time-Mapping-Software

In the present world, servicing of vehicles in automotive workshop takes more time due
to unnecessary idle time. Customers are the main priority of any industry but delay in getting
vehicles which may lead to decrease in productivity in service makes a bad impression
to the customers. A preliminary literature survey has been conducted in the domain at
various topics like improvement of productivity in automotive sector, Work and time study,
Scheduling and routing in industrial floors, time management in flow lines. In the service
centers when the customers give their cars for servicing there is a time lag in most of
the service centers. A single day work gets postponed to 2 to 3 days which causes a bad
reputation to their respective service centers. But there is a method to diagnose this which
is collectively known as time mapping technique. Time mapping helps to identify where the
time is delayed. This time mapping is used in car washes, reception, car repairs and other
sections. This time mapping is planned to implement by generating a QR code as well
as a QR code scanner which scans the QR code placed on the automobiles which requires
servicing or repairing in the present work. For each car a unique QR code is placed on
the car so there will be no confusion when servicing. These QR codes are generated as
well as scanned by a particular or a single proposed application. After servicing of the
automobile the QR code is removed and time taken will be noted down. So it can be found
out whether the service took excess time or not. The QR code is supposed to be pasted
from the entry. The time is mapped on an excel sheet so that the management can directly
monitor and find out the time lag during the service when the QR code is scanned.So the
conclusion is that this could be a huge enhancer in the automobile industries.


Time-Mapping-Software-Application is designed for a Renault service center to track vehicles and manage jobs throughout their service lifecycle.
The core features include:

Registration of jobs for incoming vehicles
Tracking job status, entry, and exit times using QR codes
Staff and vehicle management
Web dashboards and mobile interfaces for staff usage
The goal is to time-map every vehicle’s service progress using QR codes for digital entry/exit and tracking, increasing transparency and efficiency at the service center.

Use of Python
Python is primarily used for:

Backend server: The core backend is built using Django (a Python web framework).
API endpoints and business logic: Handles requests from web/mobile clients for job registration, searching, status tracking, and reporting.
Example: views.py defines functions for job management, QR code generation, staff handling, entry/exit logging, etc.
QR code generation: Uses Python’s qrcode library to generate QR images, which are then linked to vehicle/job records.
Example: The generate_qr_code view creates and saves QR codes linked with vehicle/job data.
Database storage and queries: Manages persistent storage of vehicles, jobs, staff data (using Django ORM).
Use of Java
Java is mainly used for:

Android mobile application: Java files such as main_activity.java, generateqrcode_activity.java, and qr_scanner_activity.java implement the mobile interface for staff.
QR code actions on mobile: Java is used for scanning and handling QR codes using libraries like ZXing and MLKit, enabling job entry/exit by scanning vehicle QR codes.
Client-server communication: Android app sends/receives HTTP requests to/from the Django server, such as requesting QR code generation or updating job status.


