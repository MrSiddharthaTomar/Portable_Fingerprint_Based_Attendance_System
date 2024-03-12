# Portable_Fingerprint_Based_Attendance_System
A portable fingerprint-based attendance system using Raspberry Pi

This repository contains code for constructing a portable attendance system based on fingerprint recognition with a Raspberry Pi. It integrates an R307 fingerprint sensor with a Raspberry Pi model B+ using a TTL converter. The system boasts a user-friendly graphical interface allowing educators to accurately manage student attendance, preventing the occurrence of false or fabricated records. Notable features encompass fingerprint enrollment, re-enrollment, and deletion functionalities, alongside the ability to capture attendance and transmit data to a cloud server. The project harnesses Pygame for GUI development, PyFingerprint for fingerprint handling, Fernet for encryption/decryption tasks, and SQL-Connector for interfacing with SQL databases.



# Details of files present

admin.py: This file  is used to assign fingerprints of the administrator/teacher which in turn can be used for authentication when accessing some options given in the system.

data_to_upload.py: This JSON file is used to store data(section, date, time, subject code) that needs to be sent to the database.

data_to_upload.py: This  file is used to send attendance data to a database on a cloud server.

details_of_student.py: This file is used to send details of students like name, roll number, section, and uid to the database on a cloud server.

fingerprint_registration.py: This file contains the code to enroll,re-enroll, and delete the fingerprint of the student.

fingerprint_validation.py: This file contains code to take attendance by matching the fingerprints of students with stored fingerprint data.

fingerprints.json: This file is used to store uid alongside with fingerprint data of the student(in encrypted form).

jura.ttf: This file contains jura font.

main_menu.py: This file displays the main menu (various options like register fingerprint, take attendance, upload attendance, quit)of our system and provides GUI for them.

user_interface.py: This file contains various functions/methods that are frequently used in other files. Functions like authentication of admin/teacher, display message on screen, creating buttons, and other GUI-related stuff.

verified_uids.json: This JSON file is used to store attendance data(uid to student present) that needs to be sent to the database.
