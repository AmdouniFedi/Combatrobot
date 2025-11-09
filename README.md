# Combatrobot

Combatrobot is an Arduino-based robotic project that combines movement control, obstacle detection, and servo-actuated mechanisms such as a gun, trigger, and camera. The robot can move in multiple directions, detect obstacles, and control various servo motors for interactive tasks.

## Features
- Four-wheel movement control (forward, backward, left, right, stop)
- Obstacle detection using a digital sensor
- Servo-controlled mechanisms:
  - Gun servo
  - Trigger servo
  - Camera servo
- Serial communication for remote control commands

## Hardware Requirements
- Arduino Uno or compatible board
- 4 DC motors for movement (connected via pins 8, 10, 11, 12)
- Servo motors:
  - Gun servo (pin 9)
  - Trigger servo (pin 6)
  - Camera servo (pin 5)
- Obstacle detection sensor (digital input pin 3)
- Motor driver module (H-Bridge or equivalent)
- Jumper wires and power supply

## Wiring
- **Motors**
  - Rear motor: m11 → pin 12, m12 → pin 11
  - Front motor: m21 → pin 10, m22 → pin 8
- **Servos**
  - Gun servo → pin 9
  - Trigger servo → pin 6
  - Camera servo → pin 5
- **Obstacle sensor**
  - Input → pin 3

## Software Usage
1. Open the `Combatrobot.ino` Arduino sketch in the Arduino IDE.
2. Connect your Arduino board to the computer.
3. Upload the sketch to the Arduino board.
4. Use the Serial Monitor to send commands:
   - `1` → Forward
   - `2` → Left
   - `3` → Right
   - `4` → Backward
   - `5` → Stop
   - `6` → Trigger servo action
   - `7` → Gun servo action
