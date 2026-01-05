#  Traffic Rules Violation Detection System  
### Vehicle Detection and Speed Estimation using Image Processing

##  Project Overview
This project implements a **video-based traffic monitoring system** to detect moving vehicles and estimate their speed using **digital image processing techniques**. The system aims to provide a **low-cost alternative to radar-based speed detection systems** by leveraging a stationary camera and computer vision algorithms.

The solution detects vehicles from video footage, tracks them across frames, estimates their speed, captures images of speeding vehicles, and generates a summary report of traffic violations.

---

##  Objectives
- Detect moving vehicles from a stationary camera
- Track vehicles across video frames
- Estimate vehicle speed accurately
- Capture and store images of speeding vehicles
- Generate a summary of detected vehicles and violations

---

##  System Workflow
1. **Video Acquisition**
2. **Frame Differencing**
3. **Region of Interest (ROI) & Masking**
4. **Contour Detection & Object Tracking**
5. **Speed Estimation**
6. **Vehicle Image Capture**
7. **Summary Generation**

---

##  Tools & Technologies

### Programming & Libraries
- **Python**
- **OpenCV**
- **NumPy**

### Development Environment
- **Visual Studio Code**

### Hardware Requirements
- Windows 9 / 10 / 11 (64-bit)
- Minimum Resolution: 1280 × 800
- RAM: 8 GB (Recommended)

---

##  Methodology

###  Vehicle Detection
- Background subtraction is used since the camera is stationary.
- Moving vehicles are isolated using frame differencing.

###  Object Tracking
- Contour detection identifies vehicle boundaries.
- Each vehicle is assigned a unique ID and tracked across frames.

###  Speed Estimation
- Speed is calculated based on the distance traveled between frames.
- Pixel movement is converted to real-world distance using **pixels-per-meter (PPM)** calibration.
- Speed is displayed in **km/h**.

###  Image Capture
- Vehicle images are saved once speed is calculated.
- Vehicles exceeding the speed limit are stored in a separate folder.

###  Summary Report
- A text file logs:
  - Total vehicles detected
  - Individual vehicle speeds
  - Speeding violations

