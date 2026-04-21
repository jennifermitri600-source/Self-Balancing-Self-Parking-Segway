# 🤖 Self-Balancing & Self-Parking Robot

A two-wheel autonomous robot capable of real-time self-balancing and distance-based self-parking using a Fuzzy Logic control system.

Developed for **Mechatronics System Design II**.

---

## 📌 Overview

This project implements a nonlinear control system for an inverted pendulum-based robot.  
The system maintains upright balance and autonomously moves to a predefined position while remaining stable.

The project covers:
- Dynamic system modeling
- Controller design & simulation
- Embedded implementation
- Real-world testing and tuning

---

## 🛠 System Architecture

### Hardware
- Raspberry Pi (main controller)
- Arduino (sensor interface)
- MPU6050 IMU
- DC motors + motor driver
- Custom-built chassis

### Software
- MATLAB & Simulink (modeling and simulation)
- Mamdani Fuzzy Logic Controller
- Serial communication (Arduino → Raspberry Pi)
- Sensor fusion (Complementary Filter)
- Data logging & visualization

---

## 🧠 Modeling & Control

### Dynamic Modeling
- Derived equations using Newton’s Second Law
- Converted to state-space representation
- Simulated system behavior in MATLAB/Simulink

### Self-Balancing Control

Inputs:
- Tilt angle (θ)
- Angular velocity (dθ)

Output:
- Motor voltage

Implemented a Mamdani Fuzzy Inference System to stabilize the robot in real time.

To improve measurement accuracy:
- Reduced IMU drift using a Complementary Filter
- Validated readings through experimental testing

---

## 🅿 Self-Parking Strategy

After achieving stable balancing, two motion strategies were implemented:

1. **Reaction Wheel Mechanism**  
   High-RPM flywheel creates controlled tilt bias.

2. **Reference Control Method**  
   Adjusting balance reference to induce directional movement.

Distance error = Reference position – Current position

---

## 📊 Results

- Stable closed-loop response
- Minimal oscillation
- No significant angle drift
- Successful autonomous parking
- Simulation results matched hardware performance

---

## 🎥 Demo

[![Watch Demo](https://img.youtube.com/vi/MfJysFeLQrA/0.jpg)](https://youtube.com/shorts/MfJysFeLQrA?feature=share)

---

## 📷 Additional Visuals

<img width="400" height="600" alt="241507439-9570f2c9-1389-4a82-8e89-6e6acecf86a0" src="https://github.com/user-attachments/assets/bff922a9-8ca5-47d8-90be-6705c485d52e" />


---

## 📚 Skills Demonstrated

- Control Systems Engineering  
- State-Space Modeling  
- Fuzzy Logic Control  
- Sensor Fusion  
- Embedded Systems  
- MATLAB / Simulink  
- Raspberry Pi & Arduino  
- Real-Time Hardware Tuning  

---

## 👥 Team

Developed collaboratively as part of a university project.

---

## 📁 How to Run

```bash
# Clone repository
git clone https://github.com/yourusername/robot-project.git

# Open simulation files in MATLAB
# Upload Arduino code using Arduino IDE
# Run Raspberry Pi controller script
