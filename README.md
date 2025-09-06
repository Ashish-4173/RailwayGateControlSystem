 Railway Gate Control System – 8051 Assembly

This project implements an Automatic Railway Gate Control System using the 8051 microcontroller (Assembly language). The system is designed to enhance safety at railway crossings by automatically controlling the gate, traffic lights, and countdown display based on train movement.

🔹 Features

Train Detection: Two sensors (entry & exit) connected to Port 3 detect the presence of a train.

Traffic Light Control:

Green LED → Gate open (safe for vehicles).

Red LED → Gate closed (train approaching/passing).

Stepper Motor Control: Operates the railway gate (open/close) using Port 2.

Seven-Segment Display: Countdown timer for gate operation using Port 0.

Delay Routines: Timed control for lights, motor, and countdown.

🔹 Working Principle

Default State: Green light ON, gate open, display shows 0.

Train Approaching (Sensor 1 Triggered):

Red light ON, green light OFF.

Gate closes using stepper motor.

Countdown timer starts on seven-segment display.

Train Passing: Gate remains closed until Sensor 2 detects train departure.

Train Exits (Sensor 2 Triggered):

Red light OFF, green light ON.

Gate reopens using stepper motor.

Display resets to 0.

🔹 Technical Details

Microcontroller: 8051

Ports Used:

Port 0 → Seven-Segment Display

Port 1.0 & 1.1 → Traffic LEDs

Port 2.0 – 2.3 → Stepper Motor Driver

Port 3.0 & 3.1 → Sensors (Train detection)

Programming Language: Assembly (Keil uVision / 8051 IDE)

🔹 Applications

Railway crossing automation

Safety enhancement at unmanned gates

Educational projects on embedded systems
