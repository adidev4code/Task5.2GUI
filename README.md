# SIT210 – Task 5.2C

### Raspberry Pi: Changing Light Intensity Using GUI

---

## 📌 Task Overview

This project demonstrates how to control the **brightness of three LEDs** using a **Graphical User Interface (GUI)** built with Tkinter on a Raspberry Pi. The GUI includes three sliders, each linked to one LED, allowing the user to change light intensity in real time using **PWM (Pulse Width Modulation)**.

---

## 🛠️ Hardware Required

* Raspberry Pi (with OS installed)
* Breadboard
* 3 × LEDs
* 3 × 220Ω resistors
* Jumper wires
* Keyboard and mouse (for GUI interaction)

---

## 💻 Software Required

* Raspberry Pi OS (any recent version)
* Python 3 (pre-installed on Raspberry Pi)
* Tkinter (GUI library, usually pre-installed)
* RPi.GPIO library

---

## ⚙️ Hardware Setup

1. Place the three LEDs on the breadboard.
2. Connect the **positive leg** of each LED to Raspberry Pi GPIO pins (BCM mode):

   * LED 1 → GPIO 17 (physical pin 11)
   * LED 2 → GPIO 22 (physical pin 15)
   * LED 3 → GPIO 24 (physical pin 18)
3. Connect the **negative leg** of each LED to a 220Ω resistor, then to **GND**.
4. Ensure all wiring is secure and properly seated in the breadboard.

---

## 🚀 How It Works

* Each LED is controlled using **PWM** signals from the Raspberry Pi.
* A Tkinter GUI window displays **three sliders**.
* Moving a slider adjusts the **duty cycle** of PWM, which directly changes the LED brightness.
* Sliders range from **0% (OFF)** to **100% (full brightness)**.

---

## 🔧 How to Run

1. Save the project script on your Raspberry Pi as `led_gui.py`.
2. Open a terminal in the folder containing the script.
3. Run the program:

   ```bash
   python3 led_gui.py
   ```
4. A GUI window will open with three sliders. Adjust them to control LED brightness.

---

## ✅ Testing the System

* Move each slider individually to test brightness control for each LED.
* Move multiple sliders together to confirm independent control.
* Verify that LEDs respond smoothly to changes between 0–100%.

Do you want me to also add a **“Troubleshooting” section** (like what to check if an LED doesn’t light up — e.g., wiring, GPIO mismatch, polarity)? That might help you with the 3rd LED issue and look professional in the repo.
