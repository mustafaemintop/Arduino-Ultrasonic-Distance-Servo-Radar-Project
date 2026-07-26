# Arduino Ultrasonic Distance & Servo Radar

A beginner-friendly Arduino project that combines an HC-SR04 ultrasonic sensor, a servo motor, and a buzzer to scan the environment. When an object enters the critical distance threshold, the system triggers an audio warning. You can use that for robots or cars project in the future if you want.

## Demo & Circuit

https://drive.google.com/drive/folders/18v8vjLJ4sNY1U6dla2HtMcbJRe8v4p6J?usp=sharing  


## Components Used
* Arduino Uno
* HC-SR04 Ultrasonic Sensor
* SG90 Servo Motor (referred to as `engine` in the code)
* Buzzer
* 4x AA Battery Holder( if you have 2x 2x Battery Holder You can use them by connecting them in series.
* Breadboard & Jumper Wires 

---

## How It Works
1. The ultrasonic sensor continuously sends trigger pulses to measure the distance of surrounding objects.
2. If the measured distance is **greater than** the `criticalDistance` (set to 15 cm), the servo motor sweeps back and forth between 0 and 180 degrees.
3. If an object is detected **within** the critical distance, the servo stops and the system triggers a buzzer alert to warn the user.

---

## Getting Started

1. Clone the repository or download the source files.
2. Open the `.ino` file using the Arduino IDE.
3. Connect your Arduino Uno and components according to the schematic above.
4. Upload the code to your board.
