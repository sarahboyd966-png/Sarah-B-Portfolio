# Electronic Test Instrumentation and Data Acquisition Systems - ETE 4201L

Course portfolio focused on electronic measurement, instrumentation, data acquisition, sensor interfacing, analog-to-digital conversion, bridge circuits, temperature and strain sensing, and operational-amplifier signal conditioning.

## Projects

The two larger sensor projects are organized separately in the [Projects](Projects) folder.

## Laboratory Reports

### 01 - Lab 10 - Differential and Instrumentation Amplifiers

Explored differential, subtractor, and instrumentation-amplifier circuits for conditioning small sensor signals. The work examined resistor-ratio effects, superposition, differential gain, high input impedance, and the advantages of instrumentation amplifiers when interfacing with bridge-based sensors such as strain gages.

### 02 - Lab 9 - Single-Supply Op Amps for Instrumentation

Compared dual-supply and single-supply operational-amplifier behavior, including output limitations, saturation, and the need for a mid-supply reference. The lab used a virtual ground near VCC/2 to support predictable amplification in systems that do not have a negative supply rail.

### 03 - Lab 8 - Strain Gage and Load Cell Applications

Investigated strain gages and load cells as force and weight sensors. The lab connected strain sensing to Wheatstone-bridge operation, reviewed manufacturer specifications, applied known loads, measured millivolt-level bridge outputs, and examined the relationship between mechanical deformation and electrical response.

### 04 - Lab 7 - Temperature Sensors and Thermocouples

Expanded temperature-measurement work to thermocouples and practical temperature-control systems while comparing common industrial sensor types including thermistors, RTDs, IC-based sensors, and thermocouples. The report discusses thermocouple construction, reference-junction effects, cold-junction compensation, sensor characteristics, and measurement considerations.

### 05 - Lab 6B - Thermistor Digital Thermometer with LabVIEW

Used an NTC thermistor as a temperature sensor in a voltage-divider circuit and converted resistance into temperature. The work included manufacturer data, resistance-temperature relationships, curve fitting, comparison of resistor values, and LabVIEW-based calculation and visualization of a digital thermometer system.

### 06 - Lab 6A - Wheatstone Bridge and Applications

Studied Wheatstone-bridge balance, null measurements, unknown-resistance calculation, and the sensitivity of quarter-, half-, and full-bridge configurations. The report connects bridge behavior to practical instrumentation and sensor systems while considering supply drift, meter loading, and linearity.

### 07 - Lab 5B - Hardware Analog-to-Digital Converter

Implemented and tested an 8-bit analog-to-digital converter in hardware. With a 5 V full-scale range, the lab calculated quantization step size and decision thresholds, predicted digital codes, and verified the binary outputs using eight LEDs, connecting ADC theory directly to physical circuit behavior.

### 08 - Lab 5A - ADC Modeling in LabVIEW

Built a LabVIEW VI that models an ideal analog-to-digital converter. The program uses full-scale range and bit depth to calculate quantization step size, generate the staircase transfer function, determine digital counts, and visualize quantization error across the input range.

### 09 - Lab 4 - Learning LabVIEW and NI myDAQ

Established the software and hardware foundation for later data-acquisition labs by learning LabVIEW and NI measurement hardware. The lab focused on connecting physical circuits to LabVIEW so voltage and current measurements could be acquired and displayed in real time through the front panel.

### 10 - Lab 3 - Measurement Error Statistics and Kelvin Resistance

Measured a set of approximately 100 resistors using multiple instruments and both 2-wire and 4-wire Kelvin methods. The resulting data were analyzed using mean, standard deviation, spread, histogram shape, tolerance, resolution, and measurement error to compare instrument performance and demonstrate the advantages of 4-wire resistance measurement.

### 11 - Lab 2 - Digital Multimeters and Loading Effects

Examined practical digital-multimeter behavior as a voltmeter, ammeter, and ohmmeter. The lab measured voltage-divider loading, internal meter resistance, burden voltage, and the point at which instrument loading becomes small enough to have less than a one-percent effect on a circuit measurement.

### 12 - Lab 1 - Analog Meter Operation and Design

Investigated analog meter movement, full-scale current, internal resistance, and measurement sensitivity. Series multiplier resistors and parallel shunt resistors were used to create different voltage and current ranges while reinforcing meter protection, scaling, and the relationship between current, voltage, and resistance.

### 13 - Extra Credit - ADC Comparator Circuit

Built and analyzed a comparator-based circuit that demonstrates a fundamental analog-to-digital conversion concept. A variable input voltage is compared with a reference level to generate a logic output that is passed to a PIC18F microcontroller and LEDs, illustrating how multiple comparator thresholds can form the basis of a staircase digital representation.

## Tools and Methods

LabVIEW, NI data-acquisition hardware, digital and analog multimeters, oscilloscopes, function generators, Arduino-based sensing, thermistors, thermocouples, strain gages, load cells, Wheatstone bridges, operational amplifiers, ADC hardware, statistical measurement analysis, and 2-wire/4-wire resistance measurement.