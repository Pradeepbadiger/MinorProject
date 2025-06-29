# Curvature Adaptive Headlight System (CAHS)

> 🚗 *Illuminate Smarter. Drive Safer.*

## 📌 Overview

Traditional fixed headlights fall short when navigating curves at night—leaving critical areas in shadow, delaying driver response, and increasing accident risk.  
Our project addresses this by dynamically adjusting headlight direction in real-time based on detected road curvature.

This is achieved through a low-cost, vision-based embedded system that uses real-time video processing and servo-controlled headlight orientation—enhancing road visibility and vehicle safety during night-time turns.

---

##  Problem Statement

Fixed headlights fail to illuminate curved roads adequately, leading to:
- Blind spots and delayed driver response.
- 25% of fatal night crashes on curves.
- 40% of road edges unlit on bends.
- Increased risk of 4x on curves compared to straight roads.

**Goal:** Create an adaptive headlight system that tracks road curvature and adjusts beam direction using computer vision and embedded control.

---

##  Objectives

-  Detect lane curvature using real-time computer vision.
-  Adjust headlights dynamically using servo motors.
-  Build a cost-effective and compact prototype.
-  Improve visibility and reduce night-time curve-related crashes.

---

##  Hardware Components

| Component         | Role                                      |
|------------------|-------------------------------------------|
| Raspberry Pi 5    | Main processing unit                      |
| IP Webcam         | Road video capture                        |
| 2x SG90 Servo     | Rotates headlights based on curvature     |
| High-Brightness LED | Represents adjustable headlights         |
| Toy Car Chassis   | Hardware prototype base                   |
| Jumper Wires      | Electrical connections                    |

---

##  Software & Tools

- **Python** – primary programming language
- **OpenCV** – computer vision and image processing
- **NumPy, Matplotlib** – data processing & visualization
- **PWM Libraries** – to drive the servo motors
- **Raspberry Pi OS** – embedded platform environment

---

##  System Architecture

1. **Input Capture:** Webcam captures live video feed of the road.
2. **Preprocessing:** Grayscale conversion, Gaussian blur, Canny edge detection.
3. **Lane Detection:** Hough Line Transform to detect lane lines.
4. **Curvature Estimation:** Determine curvature angle from lane orientation.
5. **Servo Control:** Convert curvature angle to PWM signal to rotate headlight.
6. **Feedback Loop:** System continuously adapts in real time (~120ms response).

---

##  Results

| Metric                | Value               |
|-----------------------|---------------------|
| System Response Time  | 100–130 ms          |
| Visibility Gain       | >45% on curved roads|
| Reaction Delay Reduced| ~0.5 seconds        |
| Beam Accuracy         | High (curve tracking)|
| Cost                  | ₹2000 (approx.)     |

---


---

##  Future Enhancements

-  AI-based curvature prediction using deep learning
-  Real-vehicle deployment with motorized headlights
-  Environment-adaptive intensity control (rain, fog)
-  Integration with autonomous navigation systems

---

##  Contributors

- **Ayan N. Sayed** 
- **Manjunath D.**  
- **Pradeep U. B.**  
- **Vishwanath H.**  
 *Mentor:* **Prof. Amit R. T.** (School of Electronics & COmmunication Engineering, KLE Technological University, Hubballi)


