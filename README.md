# RF-ID-System
# Servo Motor Control with RFID - Arduino Project

This project demonstrates how to control a servo motor using RFID authentication with an Arduino. When a valid RFID tag is detected, the servo motor is activated, simulating actions such as unlocking a door or granting access.

## 🛠️ Hardware Required

- Arduino Uno (or compatible board)
- RC522 RFID Reader
- Servo Motor (e.g., SG90)
- RFID Tags or Cards
- Jumper wires
- Breadboard
- Power supply (USB or external)

## ⚙️ How It Works

1. The RFID reader scans nearby tags.
2. If the UID of the tag matches a pre-authorized UID, the servo motor rotates to an "open" position.
3. After a short delay, the servo returns to its default "closed" position.
4. Unauthorized tags are ignored or trigger a different response.

## 📁 File Structure

- `servo_rfid.ino` - The main Arduino sketch implementing RFID-based servo control.

## 🔧 Setup Instructions

1. Connect the RC522 RFID reader to the Arduino as follows:

   | RC522 Pin | Arduino Pin |
   |-----------|-------------|
   | SDA       | D10         |
   | SCK       | D13         |
   | MOSI      | D11         |
   | MISO      | D12         |
   | GND       | GND         |
   | RST       | D9          |
   | 3.3V      | 3.3V        |

2. Connect the servo motor's:
   - **Signal** to D3 (or your chosen PWM pin)
   - **VCC** to 5V
   - **GND** to GND

3. Upload `servo_rfid.ino` to your Arduino using the Arduino IDE.

## 🧪 Demo

Upon scanning an authorized RFID tag:
- The servo unlocks (rotates).
- After a delay, it locks again (returns to default).

THANKYOU!!!

