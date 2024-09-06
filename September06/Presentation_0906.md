----
marp: true
theme: uncover
backgroundColor: black
color: white
paginate: true  # Optional: Add page numbers
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
  section {
    font-size: 14px;
  }
  h1 {
    font-size: 24px;
  }
  h2 {
    font-size: 20px;
  }
  h3 {
    font-size: 18px;
  }



----
# ECE4820: Senior Design II Project Overview

**Members**
- Dylan-Matthew Garza
- Daniel Baker
- Rohullah Sah

**Advisor**
 Dr. Janos Grantner

**Sponsor**
 ZF Group

**Date:** September 06 2024


----
## Project Specifications


<div class="columns">
<div>

### Devices Under Test (1st Model)

- Brake Signal Transmitter
    - PWM output for brake signal to make sure brakes are working within specifications
- Pressure Sensor
    - Voltage output proportional to pressure applied
- Wear Sensor
    - Voltage output proportional to brake pad wear
- Electronic Stability Control Module
    - Read from the module CAN data frame to check module functionality
- String Potentiometer
    - Determine the wear of the brake pads for alignment with production specifications
    - Determine the stroke of the brake pedal for alignment with production specifications



### Communication Layer

- WebSocket real-time data
- HTTP request methods
- JSON data handling
- XML/CSV transfers


</div>
<div>

### I/O Interfaces

- PWM (Brake Signal Transmitter)
    - Frequency: 200 ± 10 Hz
    - Voltage: 8-32V DC
    - Duty Cycle: 12.5% - 87.5%

- Analog
    Continuous Wear Sensor: 0.5V - 4.5V, 37 mm range
    Pressure Sensor: 0.5V - 4.5V, 0-10 bar range
    String Potentiometer: 0.5V - 4.5V, 37.5 mm range

- CAN (Electronic Stability Control Module)
    - Protocol: CAN 2.0A
    - Baud Rate: 500 kbaud

### Test Device Core
- ARM Cortex A7
- ARM Cortex M4
- NAND Flash w/ Embedded Linux
- Wi-Fi module
- Shared memory


</div>
</div>

----
## Block Diagram

![height:600px](block_diagram.drawio.png)
*Comprehensive block diagram of all involved development tools and 
hardware and developed software components to be implemented
along with the interactions.*

