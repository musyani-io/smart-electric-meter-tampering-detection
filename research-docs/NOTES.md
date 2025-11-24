# SUMMARY FROM THE RESEARCH

## REQUIRED TO KNOW

- [x] Which type of meters are used by TANESCO? (They buy from EDMI) => They use EDMI meters since they are believed to be long-lasting and tamper proof.
- [x] Is that meter type consistent in the whole country? => Currently no, but there's a campaign (Oct, 2025) to shift all meters (WASION and INHEMETER) to EDMI meters all over the country.
- [x] How do they work? (Measuring the units, communication to user and their servers) => Mostly use RF frequency communication _(433MHz)_ between each other to form a network up to the server (urban areas), use PLC or GSM for rural areas.
- [x] Is that particular meter type secured against tampering? If no, which ways tampering techniques affects it? => Yes, they can be tampered with. No critical information yet on tampering them.
- [ ] How can that vulnerable type (still commonly used) be acquired (bought) for demonstration?
- [ ] Can the techniques be prevented? If yes, how?

## TAMPERING TECHNIQUES

### POINTS

- **Partial Earth Faults**: Live is connected to ground instead of neutral, hence the part of current is diverted to ground making return (Neutral) current less than phase current.

- **Double Feeding**: Electric appliances (consumer's tools) are connected after the feeder but before the meter to escape the measurement of their usage.

- **Magnetic inteference**: Strong enough magnets can saturate the measuring coils to a point that they 'blind' them, hence inducing errors in measurements.

- **Physical Bypass**: Most common use of jumpers to skip out the meter by connecting jumper wires from the source to the inlet of the individual premises. In addition to this, a neighbour can inject his/her wire from other's house to navigate around fixing his/her own individual meter (mainly due to high connection expenses and existence of low cost _vishoka_)

- **Missing neutral connection**: Accidental or intentional disconnection of neutral line induces error in meter's measurements.

- **External factors (high voltage, chemical injection)**: These factors primary cause is disruption of measuring circuit purposely to alter the measurements.

- **Firmware Hacking**: This can be meter reprogramming to tamper with the variable calculations in the smart meter's MCU.

- **Communication Interference**: Eavesdropping, Man In the Middle (MIM), Replay (or Injection) and DOS can affect the signals to and from the utility and service center which in turns may affect alerts and even data logging.

- **Time manipulation (Special Case)**: For meters which alter their measurements for peak hours and normal hours, users tend to change their time to get the lowest billing as possible.

### THEIR REFERENCES

- <https://www.eetimes.com/prevent-tampering-in-energy-meters/>

- <https://www.allegromicro.com/en/insights-and-innovations/technical-documents/hall-effect-sensor-ic-publications/vertical-hall-tamper-detection#:~:text=One%20method%20employed%20in%20tampering,current%20is%20flowing%20through%20it>

- <https://circuitdigest.com/microcontroller-projects/an-iot-based-smart-ac-electricity-meter-with-tamper-protection#:~:text=4.%20Hall,tampering%20applications%20within%20the%20meter>

## TAMPERING SOLUTIONS

### POINTS

- **On Partial Earth Faults**: Explanations to follow

### THEIR REFERENCES

- <https://www.eetimes.com/prevent-tampering-in-energy-meters/>

- Abana, Ertie. (2019). Anti-Tampering Device for Residential Energy Meter. International Journal of Recent Technology and Engineering (IJRTE). 10.35940/ijrte.C6247.118419.
