# Microcontrollers - ECE 3301

Course portfolio focused on PIC18F4321 microcontroller programming, embedded hardware interfacing, assembly and C development, digital I/O, interrupt-driven control, display interfacing, and an embedded computer-vision tracking project.

## [01 - Mechanical Eyeball - AI Camera Tracking System](./01%20-%20Mechanical%20Eyeball%20-%20AI%20Camera%20Tracking%20System.pdf)

Designed and implemented a low-cost real-time mechanical camera tracking system that combines embedded AI, computer vision, microcontroller control, and a two-axis servo mechanism. The system uses a Raspberry Pi 5 and Raspberry Pi Camera Module v3 to acquire live video and detect a person, while an Arduino Uno controls two SG90 servo motors for pan and tilt. The software pipeline used Python, ONNX Runtime, and a lightweight Ultralytics YOLO model to obtain target bounding-box coordinates. Those coordinates were compared with a defined center region, creating a dead-zone style controller: when the detected person moved outside the acceptable horizontal or vertical range, the Raspberry Pi generated directional correction signals and the Arduino repositioned the camera to return the target toward the center of the frame.

The project required integration across multiple hardware and software platforms rather than operating as a single-board demonstration. Manual WASD control was implemented before autonomous tracking, then the design progressed to Raspberry Pi-to-Arduino communication and closed-loop visual tracking. Direct servo control from the Raspberry Pi produced unstable or twitchy motion, so servo actuation was moved to the Arduino. UART communication was also attempted but did not reliably deliver the control commands, so the final architecture used dedicated Raspberry Pi GPIO outputs connected to Arduino digital inputs to communicate left, right, up, and down correction states. Our team also evaluated the Raspberry Pi AI Hat+ / Hailo accelerator for person detection; although detection worked, the required bounding-box coordinate output was not available in the needed form, so the tracking logic was moved to ONNX Runtime.

Mechanical development included multiple pan-tilt stand concepts and camera configurations. An early stand was modeled in OnShape for a GoPro-style camera, later iterations were modified with FreeCAD and OnShape, and the final design used the lighter Raspberry Pi Camera Module v3 to reduce servo load and simplify software integration. The report also analyzes PWM-based servo control, SG90 versus stronger metal-geared servo options, and a possible future PCA9685-based pan-tilt architecture. Testing demonstrated that the system could identify and follow a person moving across a room, while also exposing control-tuning limitations such as choppy motion at some target speeds. The project documents the complete engineering process from architecture selection and CAD/mechanical iteration through detection software, microcontroller interfacing, troubleshooting, testing, and potential applications in surveillance, autonomous robotics, search and rescue, and other systems that require a camera to maintain a moving target in its field of view.

[Project demonstration video](https://youtu.be/xeIDUJbMzKM)

## [02 - Lab 8 - LCD Interfacing with PIC18F4321](./02%20-%20Lab%208%20-%20LCD%20Interfacing%20with%20PIC18F4321.pdf)

Interfaced an Oprex DMC16249 LCD with the PIC18F4321 and developed PIC18F assembly routines for LCD initialization, command transmission, character output, timing delays, and display clearing. Digital inputs on PORTC controlled when the text “PIC18F” was displayed, while the LCD data and control lines were driven through PIC I/O ports. The work required adapting the physical circuit to the available 14-pin LCD, configuring input/output directions, masking switch inputs, and coordinating multiple assembly subroutines to control the display.

## [03 - Lab 7 - Interrupt I-O Using Assembly and C](./03%20-%20Lab%207%20-%20Interrupt%20I-O%20Using%20Assembly%20and%20C.pdf)

Implemented interrupt-driven I/O on the PIC18F4321 using both assembly and C. An LM339 comparator generated a hardware event through INT1, allowing the microcontroller to respond through an interrupt service routine rather than continuously polling the input. The lab covered interrupt configuration, port direction, main-program and ISR structure, hardware stack behavior, comparator interfacing, and the practical difference between polling and event-driven embedded control.

## [04 - Lab 6 - Polled I-O Using Assembly and C](./04%20-%20Lab%206%20-%20Polled%20I-O%20Using%20Assembly%20and%20C.pdf)

Built a conditional I/O system using a PIC18F4321, LM339N comparator, potentiometer input, and LED output. The microcontroller repeatedly polled the comparator state and changed the LED output according to whether the adjustable voltage crossed the reference threshold. The same control behavior was implemented in PIC18F assembly and C, providing direct comparison of low-level register-based programming and compiler-based embedded development.

## [05 - Lab 5 - DIP Switch to Seven-Segment Display](./05%20-%20Lab%205%20-%20DIP%20Switch%20to%20Seven-Segment%20Display.pdf)

Designed a stand-alone PIC18F4321 hardware/software interface that reads a 4-bit value from DIP switches and displays the corresponding digit on a seven-segment display. The lab used PORTA for the switch input, PORTB for the display output, bit masking to isolate the lower input nibble, and stored seven-segment codes as a lookup table. The assembled program was programmed into the PIC using MPLAB and PICKit3 and demonstrated on a breadboard as an independent embedded system.

## [06 - Lab 4 - DIP Switch and LED I-O Interfacing](./06%20-%20Lab%204%20-%20DIP%20Switch%20and%20LED%20I-O%20Interfacing.pdf)

Interfaced DIP switches and LEDs with the PIC18F through digital I/O ports. The lab focused on configuring physical inputs and outputs and verifying the relationship between the PIC18F program and the breadboard hardware. The report includes demonstration videos for the working test code along with separate prelab and postlab explanations of both the software and physical circuit.

## [07 - Lab 3 - Assembly Subroutines and Stack Pointer](./07%20-%20Lab%203%20-%20Assembly%20Subroutines%20and%20Stack%20Pointer.pdf)

Developed a PIC18F assembly main program and subroutine while studying how CALL and RETURN instructions interact with the hardware stack. The program used FSR pointer registers, loops, arithmetic operations, and memory addressing to process a sequence of data values. MPLAB debugging was used to observe STKPTR changes during subroutine execution, reinforcing return-address handling, pointer-based memory access, and program-flow control at the assembly level.

## [08 - Lab 2 - C Programming and Debugging in MPLAB](./08%20-%20Lab%202%20-%20C%20Programming%20and%20Debugging%20in%20MPLAB.pdf)

Introduced C-language development for the PIC18F using MPLAB and the C18/XC8 toolchain. The lab compiled and debugged C programs, converted ASCII digit representations to packed BCD, added two packed BCD values, and verified the resulting variables and memory contents with the debugger. The work connected character encoding, hexadecimal representation, binary-coded decimal, bit manipulation, and embedded C debugging.

## [09 - Lab 1 - PIC18F Assembly Programming](./09%20-%20Lab%201%20-%20PIC18F%20Assembly%20Programming.pdf)

Established the PIC18F assembly-language foundation using MPLAB assembler/debugger tools. The report examines CPU and PIC18F register concepts including WREG, general-purpose registers, special-function registers, memory organization, and the STATUS carry flag. Programs used multi-byte arithmetic, data-movement instructions, direct and indirect addressing, FSR pointer registers, loops, and carry propagation, with debugger verification of register and memory results.

## Technical Scope

Raspberry Pi 5, Raspberry Pi Camera Module v3, Arduino Uno, PIC18F4321, SG90 servos, ONNX Runtime, YOLO object detection, Hailo AI acceleration evaluation, Python, Arduino C++, PIC18F assembly, embedded C, MPLAB, XC8/C18, PICKit3, GPIO communication, PWM, interrupts, polled I/O, LCD interfacing, seven-segment displays, comparator circuits, digital I/O, pointer registers, stack operation, BCD/ASCII conversion, and embedded hardware troubleshooting.
