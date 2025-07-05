# 🔔 Doorbell Circuit using Operational Amplifiers
EE254 Analog Electronics Project
Prashant Narang • Nishit Rupavatia • Piyush Raj • Sidhant Mohanty

## 📘 Overview
This project demonstrates the design, simulation, and hardware implementation of a doorbell circuit using operational amplifiers configured as a monostable multivibrator. The objective was to simulate the ringing behavior of a typical doorbell where the bell sounds for a fixed duration upon a button press.


## 🛠️ Circuit Configuration
Topology: Monostable Multivibrator using Op-Amp

## 🔄 Working Principle
On pressing the push button, the op-amp circuit enters an unstable state, causing the output to switch to a high voltage for a fixed time duration.

After 5 seconds (determined by RC time constant), the system returns to its stable low state.

The connected bulb or buzzer remains ON for 5 seconds, effectively simulating a doorbell.

## 💻 Simulation Results
State	Output Voltage
Stable (idle)	-6.33V
Unstable (ringing)	+6.33V

## 🔌 Hardware Implementation
When the button is pressed, the bulb lights up for exactly 5 seconds.

Output clamping using Zener diodes ensures voltage does not overshoot, maintaining safe operation.

## 🔍 Key Observations
A monostable multivibrator is ideal for generating the timed output needed for doorbell operation.

Without the Zener diode, the output could spike to unsafe levels (up to 30V).

The RC time constant directly controls how long the bulb stays on.

## 📷 Project Images

![image](https://github.com/user-attachments/assets/bb4bee76-0532-41ae-9ab2-550931a2f00d)

![image](https://github.com/user-attachments/assets/8c562b06-dba2-4f95-9cb3-c974c9c301ba)

![image](https://github.com/user-attachments/assets/b394db8f-697e-4e1a-bdc6-114172d5d76a)




## 🧰 Components Used
- Op-Amp: LM741

- Resistors: 10kΩ, 50kΩ

- Capacitor: 100μF

- Zener Diodes: 5.6V

- Push Button

- Bulb (or Buzzer)

## ✨ Future Enhancements
Add a debounce mechanism for the push button.

Replace LM741 with modern op-amps for better performance.

Integrate with a microcontroller for programmable ring duration.

## 🙌 Acknowledgments
Thanks to the EE254 instructors and lab team for guidance and support.

