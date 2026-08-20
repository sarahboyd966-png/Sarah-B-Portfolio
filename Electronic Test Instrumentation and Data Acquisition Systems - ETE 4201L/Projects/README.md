# ETE 4201L Projects

Two larger sensor projects from Electronic Test Instrumentation and Data Acquisition Systems are organized here separately from the regular laboratory reports.

These were team projects completed with Wesley Hwee and Mariana Rivera. The projects were previously demonstrated by video, and the original Portfolium entries provide additional project context and collaborator information.

## [Project 1](./01%20-%20Project%201.pdf) - Temperature-Controlled PWM Fan

Designed a temperature-responsive fan control system using an Arduino Nano, a 10 kOhm thermistor, an OLED display, and a 4-pin PWM fan. A 12 V input supplies the fan while an L7805 regulator provides 5 V for the control electronics. The Arduino reads the thermistor through an analog input, converts the resistance change into an ambient-temperature measurement, and uses the sensor data to control fan operation while displaying temperature and fan information. The project provided experience with sensor interfacing, analog-to-digital conversion, resistance-temperature relationships, voltage regulation, microcontroller-based control, schematic interpretation, and hardware assembly.

[Demonstration video](https://youtube.com/shorts/j8hqz1NZjKQ?feature=share)

[Original Portfolium report](https://portfolium.com/entry/ete-4201-sensor-project-1)

## [Project 2](./02%20-%20Project%202.pdf) - Heart Rate Monitor

Designed and implemented a real-time heart rate monitoring system using an Arduino Uno and a photoplethysmography (PPG) pulse sensor. The system measures changes in reflected light caused by blood-volume variation in the fingertip, conditions and samples the analog signal, detects heartbeat peaks, and calculates beats per minute. An I2C LCD provides real-time BPM output and an LED indicates each detected pulse. The project included sensor interfacing, analog signal conditioning, basic filtering and smoothing, Arduino programming, hardware integration, and comparison of the measured heart rate with a smartwatch.

[Demonstration video](https://youtu.be/jnaRiKcdwWk)

[Original Portfolium report](https://portfolium.com/entry/4201-lab-sensor-project-2)
