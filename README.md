# EXPERIMENT-04: Interfacing Analog Output With Development Board And Servo Motor

## AIM
To interface a servo motor with an Arduino UNO development board and control its angular position using programmed output signals.

## COMPONENTS REQUIRED
1. Servo Motor
2. Arduino UNO
3. USB Interfacing Cable
4. Connecting Wires

## ALGORITHM
1. Start the program.
2. Include the Servo library.
3. Create a servo object named `myservo`.
4. Attach the servo motor to digital pin 9 of the Arduino UNO.
5. Set the servo motor position to 45 degrees.
6. Wait for 1 second.
7. Set the servo motor position to 90 degrees.
8. Wait for 1 second.
9. Set the servo motor position to 135 degrees.
10. Wait for 1 second.
11. Set the servo motor position to 180 degrees.
12. Wait for 1 second.
13. Repeat the process continuously.

## PROCEDURE
1. Open Tinkercad Circuits and create a new circuit.
2. Place an Arduino UNO board and a servo motor in the workspace.
3. Connect the servo motor signal wire to digital pin 9 of the Arduino UNO.
4. Connect the servo motor VCC wire to the 5V pin of the Arduino.
5. Connect the servo motor GND wire to the GND pin of the Arduino.
6. Open the code editor and enter the Arduino program.
7. Start the simulation.
8. Observe the servo motor rotating to 45°, 90°, 135°, and 180° positions with a delay of 1 second between each position.
9. Capture screenshots of the servo motor at each angle for the output.

## PROGRAM

## DEVELOPED BY : MAHEMA A
## REGISTER NO : 212225230164
```cpp
#include <Servo.h>

Servo myservo;

void setup()
{
  myservo.attach(9);
}

void loop()
{
  myservo.write(45);
  delay(1000);

  myservo.write(90);
  delay(1000);

  myservo.write(135);
  delay(1000);

  myservo.write(180);
  delay(1000);
}
```
## OUTPUT

### Output 1 – Servo Motor at 45°

<img width="1009" height="586" alt="image" src="https://github.com/user-attachments/assets/2168d33f-e728-422d-b195-bd0c54415180" />


### Output 2 – Servo Motor at 90°

<img width="1023" height="603" alt="image" src="https://github.com/user-attachments/assets/ae155664-dac1-47a8-8052-6d65b9de96e5" />


### Output 3 – Servo Motor at 135°

<img width="1018" height="600" alt="image" src="https://github.com/user-attachments/assets/feccc705-b6c4-4dd3-9201-60247995b36a" />


### Output 4 – Servo Motor at 180°

<img width="993" height="592" alt="image" src="https://github.com/user-attachments/assets/caaa7301-c95b-4154-a4d3-313ee10ca5e6" />


## RESULT
Thus, the servo motor was successfully interfaced with the Arduino UNO development board, and its angular position was controlled at 45°, 90°, 135°, and 180° using the Arduino program.


