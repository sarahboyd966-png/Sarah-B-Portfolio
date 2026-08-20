# ETE 4201L Laboratory Reports

Laboratory work in electronic test instrumentation and data acquisition, organized from the most advanced instrumentation topics back to foundational measurement techniques.

## [01 - Lab 10 - Differential and Instrumentation Amplifiers](./01%20-%20Lab%2010%20-%20Differential%20and%20Instrumentation%20Amplifiers.pdf)
Explored differential, subtractor, and instrumentation-amplifier circuits for conditioning small sensor signals. The work examined resistor-ratio effects, superposition, differential gain, high input impedance, and the advantages of instrumentation amplifiers when interfacing with bridge-based sensors such as strain gages.

## [02 - Lab 9 - Single-Supply Op Amps for Instrumentation](./02%20-%20Lab%209%20-%20Single-Supply%20Op%20Amps%20for%20Instrumentation.pdf)
Compared dual-supply and single-supply operational-amplifier behavior, including output limitations, saturation, and the need for a mid-supply reference. The lab used a virtual ground near VCC/2 to support predictable amplification in systems without a negative supply rail.

## [03 - Lab 8 - Strain Gage and Load Cell Applications](./03%20-%20Lab%208%20-%20Strain%20Gage%20and%20Load%20Cell%20Applications.pdf)
Investigated strain gages and load cells as force and weight sensors. The lab connected strain sensing to Wheatstone-bridge operation, reviewed manufacturer specifications, applied known loads, measured millivolt-level bridge outputs, and examined the relationship between mechanical deformation and electrical response.

## [04 - Lab 7 - Temperature Sensors and Thermocouples](./04%20-%20Lab%207%20-%20Temperature%20Sensors%20and%20Thermocouples.pdf)
Expanded temperature-measurement work to thermocouples and practical temperature-control systems while comparing thermistors, RTDs, IC-based sensors, and thermocouples. The report discusses thermocouple construction, reference-junction effects, cold-junction compensation, sensor characteristics, and measurement considerations.

## [05 - Lab 6B - Thermistor Digital Thermometer with LabVIEW](./05%20-%20Lab%206B%20-%20Thermistor%20Digital%20Thermometer%20with%20LabVIEW.pdf)
Used an NTC thermistor as a temperature sensor in a voltage-divider circuit and converted resistance into temperature. The work included manufacturer data, resistance-temperature relationships, curve fitting, resistor-value comparison, and LabVIEW-based calculation and visualization of a digital thermometer system.

## [06 - Lab 6A - Wheatstone Bridge and Applications](./06%20-%20Lab%206A%20-%20Wheatstone%20Bridge%20and%20Applications.pdf)
Studied Wheatstone-bridge balance, null measurements, unknown-resistance calculation, and the sensitivity of quarter-, half-, and full-bridge configurations. The report connects bridge behavior to practical instrumentation and sensor systems while considering supply drift, meter loading, and linearity.

## [07 - Lab 5B - Hardware Analog-to-Digital Converter](./07%20-%20Lab%205B%20-%20Hardware%20Analog-to-Digital%20Converter.pdf)
Implemented and tested an 8-bit analog-to-digital converter in hardware. With a 5 V full-scale range, the lab calculated quantization step size and decision thresholds, predicted digital codes, and verified binary outputs using eight LEDs, connecting ADC theory directly to physical circuit behavior.

## [08 - Lab 5A - ADC Modeling in LabVIEW](./08%20-%20Lab%205A%20-%20ADC%20Modeling%20in%20LabVIEW.pdf)
Built a LabVIEW VI that models an ideal analog-to-digital converter. The program uses full-scale range and bit depth to calculate quantization step size, generate the staircase transfer function, determine digital counts, and visualize quantization error across the input range.

## [09 - Lab 4 - Learning LabVIEW and NI myDAQ](./09%20-%20Lab%204%20-%20Learning%20LabVIEW%20and%20NI%20myDAQ.pdf)
Established the software and hardware foundation for later data-acquisition labs by learning LabVIEW and NI measurement hardware. The lab focused on connecting physical circuits to LabVIEW so voltage and current measurements could be acquired and displayed in real time through the front panel.

## [10 - Lab 3 - Measurement Error Statistics and Kelvin Resistance](./10%20-%20Lab%203%20-%20Measurement%20Error%20Statistics%20and%20Kelvin%20Resistance.pdf)
Measured approximately 100 resistors using multiple instruments and both 2-wire and 4-wire Kelvin methods. The data were analyzed using mean, standard deviation, spread, histogram shape, tolerance, resolution, and measurement error to compare instrument performance and demonstrate the advantages of 4-wire resistance measurement.

## [11 - Lab 2 - Digital Multimeters and Loading Effects](./11%20-%20Lab%202%20-%20Digital%20Multimeters%20and%20Loading%20Effects.pdf)
Examined practical digital-multimeter behavior as a voltmeter, ammeter, and ohmmeter. The lab measured voltage-divider loading, internal meter resistance, burden voltage, and the point at which instrument loading becomes small enough to have less than a one-percent effect on a circuit measurement.

## [12 - Lab 1 - Analog Meter Operation and Design](./12%20-%20Lab%201%20-%20Analog%20Meter%20Operation%20and%20Design.pdf)
Investigated analog meter movement, full-scale current, internal resistance, and measurement sensitivity. Series multiplier resistors and parallel shunt resistors were used to create different voltage and current ranges while reinforcing meter protection, scaling, and the relationship between current, voltage, and resistance.

## [13 - Extra Credit - ADC Comparator Circuit](./13%20-%20Extra%20Credit%20-%20ADC%20Comparator%20Circuit.pdf)
Built and analyzed a comparator-based circuit that demonstrates a fundamental analog-to-digital conversion concept. A variable input voltage is compared with a reference level to generate a logic output passed to a PIC18F microcontroller and LEDs, illustrating how multiple comparator thresholds can form the basis of a staircase digital representation.

## Tools and Methods
LabVIEW, NI myDAQ/data-acquisition hardware, digital and analog multimeters, oscilloscopes, function generators, thermistors, thermocouples, strain gages, load cells, Wheatstone bridges, operational amplifiers, ADC hardware, PIC18F microcontrollers, statistical measurement analysis, and 2-wire/4-wire resistance measurement.
