🎨 Color Sorting Bot
🔍 Overview

The Color Sorting Bot is an Arduino-based project designed to automatically detect and separate objects based on their color. Using a TCS3200 color sensor, Arduino Uno, and a servo motor, the bot identifies the color of each object and sorts it into the correct container.

⚙️ Components Used

🧠 Arduino Uno

🎨 TCS3200 Color Sensor

⚙️ Servo Motor (SG90 / MG90S)

🔋 Power Supply (9V or external battery pack)

🧩 Connecting wires & breadboard

🧱 Sorting mechanism / chassis

🧰 Working Principle

The color sensor detects the color of an incoming object.

The detected color values (RGB) are sent to the Arduino Uno.

The Arduino processes the data and determines the color category.

The servo motor rotates to a specific position corresponding to the detected color bin.

The object is released into the correct section.

🔄 Algorithm Flow
Start
│
├── Initialize color sensor and servo
├── Detect color (read RGB values)
├── Compare RGB values with thresholds
├── Identify color (e.g., Red / Green / Blue)
├── Move servo to corresponding bin position
└── Return servo to initial position

🔌 Circuit Connections
Component	Arduino Pin	Description
TCS3200 S0	D2	Frequency scaling
TCS3200 S1	D3	Frequency scaling
TCS3200 S2	D4	Color filter control
TCS3200 S3	D5	Color filter control
TCS3200 OUT	D6	Sensor output
Servo Signal	D9	PWM control pin
VCC	5V	Power supply
GND	GND	Common ground
