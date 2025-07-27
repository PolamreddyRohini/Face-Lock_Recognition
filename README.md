# 🔒 FaceLock – A File Locker System Using Facial Recognition

This project implements **FaceLock**, a biometric-based file locker system that uses facial recognition to unlock or lock sensitive files. It replaces traditional passwords with a more secure, intuitive, and hands-free method of authentication using Python.

## 📌 Problem Statement

Traditional passwords are vulnerable to brute-force attacks, phishing, and are often forgotten or reused. This leads to compromised data privacy and a poor user experience. FaceLock solves this by using facial recognition to authenticate access to files, ensuring security with ease of use.

## 🧠 Abstract

FaceLock leverages:
- **OpenCV** for webcam and image handling
- **DeepFace** (with RetinaFace backend) for face recognition
- **Python Cryptography (Fernet)** for file encryption/decryption

The system captures a real-time photo from the webcam, compares it with a reference image, and grants access only on a successful match.

## 🛠️ Modules Overview

1. **Webcam Capture Module** – Takes a real-time snapshot using the webcam.
2. **Face Detection & Recognition** – Uses DeepFace with RetinaFace for identity verification.
3. **Authentication Decision** – Grants or denies access based on face match.
4. **File Encryption/Decryption** – Encrypts/Decrypts files using Fernet (symmetric encryption).
5. **Security Measures** – Cleans up temporary images, provides terminal notifications.

## 🧱 System Architecture

User Webcam
↓
Face Detection (DeepFace + RetinaFace)
↓
Verification (Match / No Match)
↓
[Match] → Decrypt / Encrypt File
[No Match] → Deny Access & Notify


## 💻 Tech Stack

| Component             | Technology Used                         |
|-----------------------|------------------------------------------|
| Programming Language  | Python                                   |
| Face Detection        | OpenCV, RetinaFace                       |
| Face Recognition      | DeepFace                                 |
| File Encryption       | Cryptography (Fernet)                    |
| IDE                   | Visual Studio Code                       |
| OS                    | Windows 10 or later                      |
| Camera                | Any standard webcam                      |

## 🔐 Proposed Algorithm

1. Start the application and webcam.
2. Capture a real-time photo.
3. Compare it with the reference image.
4. If match:
   - If file is encrypted → decrypt.
   - If file is decrypted → encrypt.
5. If no match → deny access.
6. Notify user.
7. Delete temp images.

## 📸 Output

- Real-time face scanning via webcam.
- Locks or unlocks files securely based on face verification.
- Provides terminal-based notifications.

## 🔮 Future Improvements

- Multi-user face authentication
- Mobile app version
- Liveness detection to avoid spoofing
- GUI-based interface
- Cloud-based secure file access
- Logging and email/SMS alerts on failed attempts

## ✅ Conclusion

**FaceLock** is a robust AI-powered biometric file security system using facial recognition. It removes the need for passwords, adds convenience, and enhances security using deep learning and encryption. Perfect for securing personal or enterprise-level data in real-time.

