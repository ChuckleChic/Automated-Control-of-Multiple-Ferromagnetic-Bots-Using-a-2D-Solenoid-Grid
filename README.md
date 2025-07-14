# Automated Control of Multiple Ferromagnetic Bots Using a 2D Solenoid Grid

##  Overview
This repository contains the detailed report of an 8-week research internship conducted at the **M2D2 Lab, IISc Bengaluru**, focused on developing an **autonomous control system** for multiple ferromagnetic bots using a 2D solenoid grid.

The system replaces manual coil activation with a vision-based, automated control mechanism using **Python algorithms**, **Arduino microcontrollers**, and **camera-based tracking**. This setup enables coordinated tasks like **shape transformation**, **navigation through obstacles**, and **object manipulation**.

---

##  Problem Statement
Global magnetic field-based control systems fail to provide independent control over individual bots. This project aims to overcome that challenge by:
- Automating the control of bots using **localized solenoids**.
- Designing **vision-based algorithms** for path planning.
- Implementing **real-time coil activation** using serial communication with Arduino.

---

##  Experimental Setup
- A **grid of solenoids** generates localized magnetic fields.
- Overhead **camera system** tracks bots in real-time.
- Bots consist of **ferromagnetic balls** in spring-loaded holders with **Teflon feet** for smooth movement.
- An **automatic braking system** enables precise control by using friction.

---

## ⚙ Core Functional Modules
1. **Camera Calibration & Position Measurement**
2. **Shape Formation Algorithms**: Square, Diamond, I-shape, C-shape, O-shape
3. **Translation & Rotation Modules**
4. **Object Grasping Logic**
5. **Coil Mapping & Activation through Arduino**
6. **Real-time Vision Feedback Loop**

---

##  Motion Planning Workflow
1. **Bot Detection** and center calculation.
2. **Target Position Assignment** based on vector angle analysis.
3. **Magnetic Actuation** using nearest effective coils.
4. **Continuous Position Update** for iterative corrections.
5. **Verification & Task Completion** using real-time feedback.

---

##  Challenges & Solutions
| Challenge | Solution |
|----------|----------|
| Faulty coils and loose connections | Rerouted connections via alternative green boards |
| Camera calibration error | Refined distortion model and camera settings |
| Bots failing to respond | Added frame-based position feedback and correction logic |
| Oscillating bot behavior | Introduced tolerance thresholds and error correction |
| Lighting interference | Dynamically adjusted OpenCV thresholding |

---

##  Experimental Demonstration
The final implementation demonstrated:
- Translation and rotation of bots in complex paths.
- Real-time object grabbing using shape transformation.
- Adaptive control in constrained environments.

---

##  Future Work
- Obstacle detection using advanced vision techniques.
- Adaptive shape selection based on obstacle geometry.
- Scaling to larger bot arrays and grids.

---

## 👤 Author
**Priya Jha**  
Research Intern  
Department of Mechanical Engineering  
Indian Institute of Science (IISc), Bengaluru  

---

## 📌 Citation
If you use or refer to this project, please cite the following paper that inspired this work:
> Bhat S, Ananthasuresh GK. *Actuation of ferrobots in a plane for independent and swarm motion using a grid of electromagnets.* 2023 International Conference on MARSS.

---

## 🛠 Technologies Used
- Python (OpenCV, NumPy)
- Arduino (PWM control via PCA9685)
- Serial Communication (pySerial)
- Camera Calibration Techniques

---

## 📬 Contact
For queries, feel free to connect via LinkedIn or email.

---

