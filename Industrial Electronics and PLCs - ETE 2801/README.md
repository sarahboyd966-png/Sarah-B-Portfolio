# Industrial Electronics and PLCs - ETE 2801

Course portfolio focused on industrial electrical systems, three-phase power, transformers, electromechanical control, PLC programming, motor starters, isolation, DC and AC machines, PWM motor control, and industrial drive concepts. Reports are ordered from the most advanced laboratory work to the earlier foundational labs, with the two in-class demonstration records placed last.

## [01 - Lab 12 - Three-Phase Induction Motors](./01%20-%20Lab%2012%20-%20Three-Phase%20Induction%20Motors.pdf)

Investigated the operation and performance of a three-phase induction motor using mechanical and electrical measurements. The lab recorded torque, speed, current, real power, reactive power, apparent power, and power factor to evaluate motor behavior and efficiency under changing load. It also examined industrial variable-frequency/variable-speed control, the relationship between supply frequency and synchronous speed, non-contact speed verification with a stroboscopic light, and direction reversal by changing the phase sequence. The setup additionally used the three-phase motor as a prime mover for a DC generator, connecting motor-drive behavior with electromechanical energy conversion.

## [02 - Lab 11 - PWM Motor Control and H-Bridge](./02%20-%20Lab%2011%20-%20PWM%20Motor%20Control%20and%20H-Bridge.pdf)

Applied pulse-width modulation to practical motor control and verified the relationship between duty cycle and average voltage with a function generator and oscilloscope. The report compares predicted and measured PWM waveforms, examines sine-PWM concepts, and connects average applied voltage to motor speed. The final hardware implementation used an L298N electronic H-bridge so PWM could control motor speed while logic inputs controlled direction, providing experience with modulation, scope measurements, motor-driver interfacing, and efficient electronic speed control.

## [03 - Lab 10 - DC Motor Load Torque Speed and Efficiency](./03%20-%20Lab%2010%20-%20DC%20Motor%20Load%20Torque%20Speed%20and%20Efficiency.pdf)

Characterized a DC motor by measuring voltage, armature current, torque, speed, input/output power, and efficiency over a range of mechanical loads. The analysis connected motor equations to measured behavior and showed the inverse relationship between load torque and speed, the increase in current required as torque rises, and the change in operating efficiency across the motor's usable range. The report also discusses rated operating points, stall-current concerns, magnetic flux, brushes, armature behavior, and the conversion between electrical input and mechanical output power.

## [04 - Lab 9 - PLC Timers and Counters](./04%20-%20Lab%209%20-%20PLC%20Timers%20and%20Counters.pdf)

Implemented timer and counter functions used in programmable-logic control. The work examined on-delay and off-delay timing behavior, counter presets and accumulated values, rising-edge event counting, reset logic, and the difference between measuring elapsed time and counting discrete process events. Physical PLC circuits were built and demonstrated, connecting ladder-logic instructions with real input/output behavior and the CLICK programming environment.

## [05 - Lab 8 - PLC Motor Starter and H-Bridge](./05%20-%20Lab%208%20-%20PLC%20Motor%20Starter%20and%20H-Bridge.pdf)

Recreated a forward/reverse motor-starter control system with a PLC, physical switches, and relay outputs. The PLC interpreted a normally closed stop input plus normally open forward and reverse commands, replacing portions of the earlier hard-wired relay logic with programmed control in CLICK software while external relays provided output switching. The lab also analyzed a transistor-based electronic H-bridge and documented the practical wiring and common-connection troubleshooting required to obtain correct relay behavior. This report demonstrates the transition from relay-only industrial control to programmable automation.

## [06 - Lab 7 - Optocouplers and Electrical Isolation](./06%20-%20Lab%207%20-%20Optocouplers%20and%20Electrical%20Isolation.pdf)

Built and tested several optocoupler configurations to study electrical isolation between control and power sections. Devices included IC-style optoisolators, slotted opto-interrupters, and reflective optocouplers, with test circuits used to examine LED drive current, phototransistor/open-collector behavior, and isolated signal transfer. The lab emphasizes why optical isolation is useful at PLC and industrial-control interfaces where high voltage, transients, and electrical noise must be kept away from sensitive low-voltage electronics.

## [07 - Lab 6 - Relay Motor Control and Forward-Reverse Starter](./07%20-%20Lab%206%20-%20Relay%20Motor%20Control%20and%20Forward-Reverse%20Starter.pdf)

Designed and constructed relay-based motor-control circuits while learning to read industrial ladder diagrams. The work progressed from basic relay logic to a motor starter with separated control and motor-power sections and then to a forward/reverse starter using multiple relays. Safety and control behavior were central to the design, including normally open and normally closed pushbuttons, seal-in/holding behavior, prevention of automatic restart after power restoration, and relay arrangements used to reverse motor direction.

## [08 - Lab 5 - Industrial Control Devices Relays Solenoids and Contactors](./08%20-%20Lab%205%20-%20Industrial%20Control%20Devices%20Relays%20Solenoids%20and%20Contactors.pdf)

Surveyed and tested common industrial control hardware including switches, indicators, electromechanical relays, solenoids, rheostats, and contactors. The report uses manufacturer datasheets to compare contact configurations, voltage/current ratings, environmental ratings, mounting, lifetime, coil requirements, and application limits. Hands-on relay testing examined pull-in and drop-out behavior and polarity sensitivity, while later sections studied solenoid actuation and higher-current contactors used for industrial power switching. The lab developed practical component-selection and datasheet-reading skills in addition to circuit construction.

## [09 - Lab 4 - Transformer Wiring and Voltage Regulation](./09%20-%20Lab%204%20-%20Transformer%20Wiring%20and%20Voltage%20Regulation.pdf)

Experimentally studied transformer construction, winding identification, turns ratio, voltage/current relationships, and multi-winding configurations. Continuity and winding resistance measurements were used to identify the primary and secondary coils, and measured primary/secondary voltages were compared with transformer ratio relationships. Series, parallel, and center-tapped configurations were examined to understand tradeoffs between voltage and current capability, voltage regulation, electrical isolation, and the relationship to residential three-wire 120/240 V distribution.

## [10 - Lab 3 - Three-Phase Power Wye and Delta Loads](./10%20-%20Lab%203%20-%20Three-Phase%20Power%20Wye%20and%20Delta%20Loads.pdf)

Analyzed balanced and unbalanced three-phase resistive loads in both Wye and Delta configurations. Measurements of phase voltage, line voltage, line current, and neutral current were compared with detailed phasor and impedance calculations using a LabVolt three-phase source and measurement equipment. The report examines the sqrt(3) line/phase relationships, 120-degree phase displacement, neutral-current behavior under balanced versus unbalanced loading, and the effect of connecting or removing the Wye neutral. A step-by-step calculation guide is included as part of the report.

## [11 - In-Class Demonstration - EMR vs SSR Relay Arcing](./11%20-%20In-Class%20Demonstration%20-%20EMR%20vs%20SSR%20Relay%20Arcing.pdf)

Technical response to an in-class comparison of electromechanical relays and solid-state relays. The demonstration focused on visible contact arcing in mechanical switching, the resulting contact wear and pitting, slower switching response, and the potential for electrical noise and radio-frequency interference. The write-up contrasts this behavior with solid-state switching, emphasizing the absence of mechanical contacts and arcing as an important SSR advantage.

## [12 - In-Class Demonstrations - Industrial Machines and Three-Phase Waveforms](./12%20-%20In-Class%20Demonstrations%20-%20Industrial%20Machines%20and%20Three-Phase%20Waveforms.pdf)

Photographic documentation from the final ETE 2801 laboratory session. The images show industrial electrical-machine and power-training hardware, including a transformer panel, variable-capacitor hardware, a squirrel-cage induction motor and electrodynamometer setup, along with an oscilloscope displaying multiple phase-shifted sinusoidal waveforms. Several additional photographs are identified in the original submission as a Parker demonstration. Because no formal report was required for this session, this entry is retained as supporting documentation rather than a full laboratory analysis.

## Technical Scope

Three-phase Wye and Delta systems, phasor calculations, neutral current, transformers, center taps, relays, contactors, solenoids, optocouplers, ladder logic, PLCs, CLICK programming, timers, counters, motor starters, forward/reverse interlocking, transistor and integrated H-bridges, DC motors, torque-speed characteristics, motor efficiency, PWM, duty cycle, oscilloscopes, function generators, three-phase induction motors, variable-frequency drives, power factor, VAR/VA/W measurements, stroboscopic speed measurement, and industrial electrical troubleshooting.