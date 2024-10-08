## ESP32 Easy Coding Board Stone Thrower Projects

### Code Download

[Click to download the code package](./Codes.zip).

![j6](./media/j6.png)

### 1. Button Module

![1-1](./media/1-1.png)

#### 1.1 Introduction

Button module is an input component for electronic devices, which is widely used in computers, mobile phones, home appliances and so on. It converts the physical button operation into electrical signals for reorganization and processing. It is composed of a button switch, a contact point, a conductive material and a circuit board.

#### 1.2 Schematic Diagram

![1-2](./media/1-2.png)

Pressing or releasing the button changes the state of the circuit (high level: 1, low level: 0), so as to input information. 

For example in the circuit diagram, press the button and pin 1-3 and 2-4 are connected so that the s-end is pulled down to the ground, and the button value is `0` now. Release the button, pin 1-3 and 2-4 are disconnected, and s-end is pulled up by VCC and resistor R1, so the button value is `1`.

------

#### 1.3 Parameters

Operating voltage: DC 3.3-5V

Operating temperature: -10°C ~ +50°C

Dimensions: 31.6mmx23.7mm

Interface: 3PIN interface

Output signal: digital signal



------

#### 1.4 Wiring Diagram

![1-3](./media/1-3.png)

#### 1.5 Test Code

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
2. In ![a8](./media/a8.png), drag ![a9](./media/a9.png) and set baud rate to `9600`
3. In ![a1](./media/a1.png), add ![a5](./media/a5.png) under ![a9](./media/a9.png)

![1-4](./media/1-4.png)

4. In ![a8](./media/a8.png), put ![a10](./media/a10.png) into ![a5](./media/a5.png)
5. In ![a7](./media/a7.png), drag ![a18](./media/a18.png) and set pin to IO16. And put it in the printing box of ![a10](./media/a10.png)
6. For better observation, click ![a1](./media/a1.png) and find ![a47](./media/a47.png), set delay to 0.3S

**Complete Code**

![1-5](./media/1-5.png)

**Test Result**

After uploading code, you can see the button value on the serial monitor of KidsBlock Desktop. 

Press the button and the value is `0`, and release it to change into `1`. If you cannot see the printing box, click ![a11](./media/a11.png) on KidsBlock.

![1-6](./media/1-6.png)

#### 1.5 Expansion Code

Button controls the RGB dot matrix.

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
2. In ![a3](./media/a3.png), put ![a4](./media/a4.png) under ![a2](./media/a2.png)
3. In ![a1](./media/a1.png), put ![a5](./media/a5.png) under ![a4](./media/a4.png)
4. In ![a1](./media/a1.png), find ![a6](./media/a6.png) and put it into ![a5](./media/a5.png)
5. In ![a7](./media/a7.png), drag ![a18](./media/a18.png) and set the pin to IO16; and then add it into the condition box of ![a6](./media/a6.png)

![1-7](./media/1-7.png)

6. In ![a3](./media/a3.png), drag ![a12](./media/a12.png), and modify color ![a13](./media/a13.png) to set it to red![a14](./media/a14.png). Click ![a15](./media/a15.png) and choose ![a16](./media/a16.png). Put it into “then” of ![a6](./media/a6.png)
7. In ![a3](./media/a3.png), drag ![a12](./media/a12.png) and click ![a13](./media/a13.png) to set color to red ![a14](./media/a14.png) and set display icon to ![a15](./media/a15.png). Put it into “else” of ![a6](./media/a6.png)



**Complete Code**

![KidsBlock Project-1725328227030](./media/1-8.png)

**Test Result**

After uploading the code, ESP32 Easy Coding Board shows ![a16](./media/a16.png). Press the button, and it displays ![a17](./media/a17.png).

### 2. Rotary Potentiometer

![2-1](./media/2-1.png)

#### 2.1 Introduction

Potentiometer module is essentially an adjustable resistor. When we rotate it, we change its resistance. We set up the corresponding circuit to convert the change in the resistance into a change in the voltage, which is then detected by the analog input port of the micro: bit board through the signal end.

#### 2.2 Schematic Diagram

![2-2](./media/2-2.png)

#### 2.3 Parameters

Operating voltage: DC 3.3-5V

Operating temperature: -10°C ~ +50°C

Dimensions: 35mm x 20mm x 28mm

Interface: 3PIN interface

Output signal: analog signal

#### 2.4 Wiring Diagram

![2-3](./media/2-3.png)

#### 2.5 Test Code

**Test Code**

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
2. In ![a8](./media/a8.png), drag ![a9](./media/a9.png) and set baud rate to `9600`
3. In ![a1](./media/a1.png), drag ![a5](./media/a5.png) and put it under ![a9](./media/a9.png)

![1-4](./media/1-4.png)

4. In ![a8](./media/a8.png), drag ![a10](./media/a10.png) and put it into ![a5](./media/a5.png)
5. In ![a7](./media/a7.png), drag ![a19](./media/a19.png) and set pin to IO32, and put it intot the printing content box of ![a10](./media/a10.png)
6. For better observation, click ![a1](./media/a1.png) and add a ![a47](./media/a47.png), set the delay to 0.3S

**Complete Code**

![2-4](./media/2-4.png)

**Test Result**

After uploading the code, KidsBlock Desktop serial monitor prints the analog values of the potentiometer. Rotate the potentiometer and these values change (range: 0-4095). If you cannot see the printing box, click ![a11](./media/a11.png) on KidsBlock.

![2-5](./media/2-5.png)

#### 2.6 Expansion Code

Potentiometer controls the brightness of RGB dot matrix

**Expansion Code**

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
2. In ![a3](./media/a3.png), drag ![a4](./media/a4.png) and put it under ![a2](./media/a2.png)
3. In ![a20](./media/a20.png), drag ![a21](./media/a21.png) and set variable name to `value`, and put it under ![a4](./media/a4.png)
4. In ![a1](./media/a1.png), put ![a5](./media/a5.png) under ![a21](./media/a21.png)

![2-6](./media/2-6.png)

5. In ![a20](./media/a20.png), drag ![a22](./media/a22.png) and set variable name to `value`, and put it into ![a5](./media/a5.png)
6. In ![a23](./media/a23.png), put ![a24](./media/a24.png) into ![a25](./media/a25.png)
7. In ![a7](./media/a7.png), drag ![a19](./media/a19.png) and set the pin to IO32, and put it into the first box of ![a24](./media/a24.png), modify the following box into `0`, `4095`, `0`, `255` respectively.

![2-7](./media/2-7.png)

8. In ![a3](./media/a3.png), drag ![a12](./media/a12.png) and click ![a13](./media/a13.png) to set the color to red ![a14](./media/a14.png), set the icon to ![a15](./media/a15.png), and put it under ![2-7](./media/2-7.png)

9. In ![a20](./media/a20.png), drag ![a34](./media/a34.png) and input `value`, and put it into the ![a27](./media/a27.png) of ![a26](./media/a26.png)

**Complete Code**

![2-8](./media/2-8.png)

**Test Result**

After uploading code, you may not see the ![a17](./media/a17.png) on the RGB dot matrix. Rotate the potentiometer to increase the brightness value of RGB, and the icon will show up.



### 3. Servo

#### 3.1 Introduction

The servo is a kind of position servo driver, which is mainly composed of housing, circuit board, core-less motor, gear and position detector. The receiver or microcontroller sends a signal to the servo which has an internal reference circuit that generates a reference signal with a period of 20ms and a width of 1.5ms, and compares the DC bias voltage with the voltage of the potentiometer to output voltage difference.

There are many specifications of servo, but they all contain three wires respectively in brown, red, and orange (colors may vary from brands). The brown is GND, the red is the positive power supply, and the orange is the signal line.

![3-1](./media/3-1.jpg)

The rotation Angle of the servo is controlled by adjusting the duty cycle of the PWM (pulse width modulation) signals. Theoretically, the period of the standard PWM signal is fixed at 20ms (50Hz), so the pulse width should be 1ms ~ 2ms. But in fact, it is 0.5ms ~ 2.5ms, corresponding to the servo angle of  0° ~ 180°. 

![3-2](./media/3-2.png)

#### 3.2 Parameters

Operating voltage: DC 3.3V〜5V

Operating angle range: approx. 180°(at 500→2500 μsec)

Pulse width range: 500→2500 μsec

No-load speed: 0.12±0.01 sec/60(DC 4.8V)    0.1±0.01 sec/60(DC 6V)

No-load current: 200±20mA(DC 4.8V)    220±20mA(DC 6V)

Stop torque: 1.3±0.01kg·cm(DC 4.8V)    1.5±0.1kg·cm(DC 6V)

Stop current: ≦850mA(DC 4.8V)    ≦1000mA(DC 6V)

Standby current: 3±1mA(DC 4.8V)    4±1mA(DC 6V)

#### 3.3 Wiring Diagram

![](./media/3-3.png)

#### 3.4 Test Code

**Test Code**

1. Import the servo library first. Click ![a28](./media/a28.png) and choose `Actuator`, find `Servo` library and load it.

![a29](./media/a29.png)

After loading, click ![a30](./media/a30.png) to back to the main interface.

![a31](./media/a31.png)

2. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
3. In ![a1](./media/a1.png), put ![a5](./media/a5.png) under ![a2](./media/a2.png)
4. In ![a32](./media/a32.png), drag ![a33](./media/a33.png) and set the pin to `IO14`, and angle to `0` degree, and modify the delay to `1000`(unit: ms), and put it into ![a5](./media/a5.png)
5. In ![a32](./media/a32.png), drag ![a33](./media/a33.png) and set the pin to `IO14`, and angle to `90` degree, and modify the delay to `1000` (unit: ms), and put it under the above block.
6. In ![a32](./media/a32.png), drag ![a33](./media/a33.png) and set the pin to `IO14`, and angle to `180` degree, and modify the delay to `1000` (unit: ms), and put it under the above block.

**Complete Code**

![3-4](./media/3-4.png)

**Test Result**

After uploading the code, the servo rotates from 0 degree to 90 degree and then to 180 degree with intervals of 1 second of each.

#### 3.5 Expansion Code

Potentiometer controls the servo. Their wiring connections remains unchanged.

**Expansion Code**

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)

   

2. In ![a20](./media/a20.png), drag ![a21](./media/a21.png) and set the variable name to `value`, and put it under ![a2](./media/a2.png)

3. In ![a1](./media/a1.png), put ![a5](./media/a5.png) under ![a21](./media/a21.png)

![3-5](./media/3-5.png)

5. In ![a20](./media/a20.png), drag ![a22](./media/a22.png) and input variable name `value`, and put it into ![a5](./media/a5.png)
6. In ![a23](./media/a23.png), drag ![a24](./media/a24.png) and put it into ![a25](./media/a25.png)
7. In ![a7](./media/a7.png), drag ![a19](./media/a19.png) and set the pin to IO32, and put it into the first box of ![a24](./media/a24.png), and modify the following box into `0`, `4095`, `0`, `180` respectively.

![3-6](./media/3-6.png)

8. In ![a32](./media/a32.png), drag ![a33](./media/a33.png) and set the pin to `IO14`, set the delay time to `10`(unit: ms), and put it under ![3-6](./media/3-6.png)

9. In ![a20](./media/a20.png), drag ![a34](./media/a34.png) and input variable name `value`, and put it into ![a36](./media/a36.png) of ![a35](./media/a35.png)

**Complete Code**

![3-7](./media/3-7.png)

**Test Result**

After uploading the code, rotate the potentiometer to control the rotation of the servo from 0 degree to 180 degree. You can control it to stop at any angle. 

If your stone thrower are assembled, the servo controls the thrower arm and swings may appear when the potentiometer controls the it to 90 degree.

### 4. Ultrasonic Sensor

#### 4.1 Introduction

Like bats, HC-SR04 ultrasonic sensor adopts sonar to determine the distance to objects. It provides excellent contact-less range inspection with high accuracy and stable readings. Internally, it is equipped with ultrasonic transmitter and receiver. 

In application, it is used in a wide range of electronics projects for obstacle detection and distance measurement.

#### 4.2 Parameters

Operating voltage: 3.3-5V 

Static current: <2mA

Working current: 15mA

Valid angle: <15°

Distance range: 2cm – 400 cm

Accuracy: 0.3 cm

Measuring Angle: 30 degrees

Trigger input pulse width: 10 microseconds

![4-1](./media/4-1.jpg)

#### 4.3 Wiring Diagram

![4-2](./media/4-2.png)

| VCC(red) | Trig(white) | Echo(brown) | Gnd(black) |
| :------: | :---------: | :---------: | :--------: |
|   3V3    |  P8 / io4   | P12 / io15  |    GND     |



#### 4.4 Test Code

**Build code:**

1. Import ultrasonic library first. Click ![a28](./media/a28.png) to choose `Sensor`, find `Ultrasonic` and load it.

![a37](./media/a37.png)

Successfully loaded. Click ![a30](./media/a30.png) to back to the main interface.

![a38](./media/a38.png)

2. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)
3. In ![a8](./media/a8.png), drag ![a9](./media/a9.png) and set baud rate to `9600`
4. In ![a1](./media/a1.png), drag ![a5](./media/a5.png) and put it under ![a9](./media/a9.png)

![1-4](./media/1-4.png)

4. In ![a8](./media/a8.png), drag ![a10](./media/a10.png) and put it into ![a5](./media/a5.png)
5. In ![a39](./media/a39.png), drag ![a40](./media/a40.png) and set trig to pin IO4, echo to pin IO15, and put it into the print content box of ![a10](./media/a10.png)
6. For better observation, click ![a1](./media/a1.png) to add a ![a47](./media/a47.png) and set delay to 0.5S

![4-3](./media/4-3.png)

**Test Result**

After uploading code, the serial monitor prints the distance value to the obstacles. If you cannot see the printing box, click ![a11](./media/a11.png) on KidsBlock.

![4-4](./media/4-4.png)

#### 4.5 Expansion Code

**Expansion Code**

1. In ![a1](./media/a1.png), drag ![a2](./media/a2.png)

   

2. In ![a20](./media/a20.png), drag ![a21](./media/a21.png) and name the variable to `distance`, and put it under ![a2](./media/a2.png)

3. In ![a1](./media/a1.png), drag ![a5](./media/a5.png) and put it under ![a21](./media/a21.png)

![4-5](./media/4-5.png)

5. In ![a20](./media/a20.png), drag ![a22](./media/a22.png) and modify the variable name to `distance` and put it in ![a5](./media/a5.png)
6. In ![a39](./media/a39.png), drag ![a40](./media/a40.png) and set trig to pin IO4, echo to pin IO15, and put it into the last box of ![a41](./media/a41.png)
7. In ![a1](./media/a1.png), put ![a42](./media/a42.png) under ![a43](./media/a43.png)
8. In ![a44](./media/a44.png), put ![a45](./media/a45.png) into the condition box of ![a42](./media/a42.png)
9. In ![a20](./media/a20.png), drag ![a34](./media/a34.png) and name it to `distance`, and put it into the left box of ![a45](./media/a45.png), modify the right box into `6`.

![4-6](./media/4-6.png)

10. In ![a46](./media/a46.png), find ![a48](./media/a48.png) and ![a49](./media/a49.png), put them into ![a42](./media/a42.png)

    ![4-7](./media/4-7.png)

11. At last add a delay of 0.3S under ![a42](./media/a42.png)

**Complete Code**

![4-8](./media/4-8.png)

**Test Result**

After uploading code, when the ultrasonic sensor detects a distance to the object that is lower than 6CM, the on-board buzzer emits sound. You can test by pretending to be an obstacle with your hand.



### 5. Stone Thrower

#### 5.1 Introduction

In this project, we build a stone thrower with a button module, a potentiometer, an ultrasonic sensor and servos. 

#### 5.2 Wiring Table

Connections are the same, except the servo 2. Here is the wiring table.

|      Module       |     GND     |    VCC    |      S / Echo       |       Trig        |
| :---------------: | :---------: | :-------: | :-----------------: | :---------------: |
|      button       | GND (black) | 3V3 (red) | P9 / io16 (yellow)  |                   |
|   potentiometer   | GND (black) | 3V3 (red) | P2  / io32 (yellow) |                   |
|  servo 1 (base)   | GND (brown) | 3V3 (red) | P0  / io12 (yellow) |                   |
|   servo 2 (arm)   | GND (brown) | 3V3 (red) | P1  / io14 (yellow) |                   |
| ultrasonic sensor | GND (black) | 3V3 (red) | P12  / io15 (brown) | P8  / io4 (white) |



#### 5.3 Test Code

![5-1](./media/5-1.png)

#### 5.4 Test Result

After uploading the code, rotate the potentiometer to adjust the angle of the thrower arm. 

When the distance of the obstacle in front  is less than 20CM, stones can be projected. Pressing the button to project stones. 

------



## 2.FAQ

### Q: Battery model?

A: Four AAA batteries. Please install the batteries in the correct direction rather than reverse them! For younger students, please be accompanied by your parents!

------



### Q: Error occurs when burning programs on ESP32 board?

A: 

- Please check whether the USB port number is correct.
- Please ensure the main board model is available. 

------



### Q: Expand to external modules?

A: It can expand to external modules. For details, please follow the ESP32 pin instructions to ensure external modules can normally work.

------



## 3. Resources

Keyestudio official:

[https://www.keyestudio.com/](https://www.keyestudio.com/)

Keyestudio wiki main page:

[https://wiki.keyestudio.com/Main_Page](https://www.keyestudio.com/)

Arduino official:

[https://www.arduino.cc/](https://www.keyestudio.com/)

ESP32 espressif official:

[https://www.espressif.com/](https://www.keyestudio.com/)
