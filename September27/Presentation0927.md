----
marp: true
theme: uncover
backgroundColor: black
color: cyan
paginate: true  # Optional: Add page numbers
style: |
  .columns {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }
  section {
    font-size: 18px;
  }
  h1 {
    font-size: 28px;
  }
  h2 {
    font-size: 24px;
  }
  h3 {
    font-size: 22px;
  }
    code:not([class]) {
    background-color: black;
    color: #00ff00;
    padding: 0.2em 0.4em;
    border-radius: 3px;
    font-family: monospace;
    font-size: 0.9em;
  }
  pre {
    background-color: black;
    padding: 1em;
    border-radius: 5px;
  }
  pre code {
    color: #00ff00;
    padding: 0;
  }



----
# ECE4820 Senior Design II: Presentation 3
## Gantt Chart Progress, Updated Budget Projection, Progress Report

## Members
- Dylan-Matthew Garza
- Daniel Baker
- Rohullah Sah

## Advisor
 Dr. Janos Grantner

## Sponsor

 ZF Group

**Date**: September 27 2024

----

# Gantt Chart Update (1/2)

![height:600px](../Images/Gantt_chart_all_0927.png)

----

# Gantt Chart Update (2/2)

![height:500px](../Images/Gantt_chart_done_0927.png)

----


# Budget Projections Update

![height:600px](../Images/budget_projection.png)

----

# Progress Report - Rohullah Sah (1/3)

![height:600px](../Images/rz1.jpg)

----

# Progress Report - Rohullah Sah (2/3)

![height:600px](../Images/rz2.jpg)

----

# Progress Report - Rohullah Sah (2/3)

![height:600px](../Images/rz3.jpg)

----



# Progress Report - Daniel Baker (1/)
## Implementation of BST Protocol on Cortex-M4

### Completed BST Test Protocol:
- Successfully implemented the Brake Stroke Test (BST) protocol on the Cortex-M4 processor.
- Ensured that the test adheres strictly to product specification ranges for accuracy and reliability.
- Added Test Points:
- Incorporated specific test points according to the product specifications.
- This facilitates better diagnostics and validation during testing phases.

----

# Progress Report - Daniel (2/)
## Development of Stroke Estimation Feature


- Option Without String Potentiometer:
- Developed an estimation feature within the BST code to calculate the brake stroke when a string potentiometer is not used.
- Enhances the system's versatility by allowing testing in different hardware configurations.

- Aimed to enable the execution of M4 programs via a click of a button on the web server.
- Focused on making the system efficient and user-friendly.

----

# Progress Report - Daniel (3/)

## Code Testing and Optimization

- Performance Validation:
- 
- Conducted thorough testing of the BST code to ensure it functions correctly within specified ranges.
- Verified the accuracy of calculations to detect pass or fail conditions.
- Code Refinement:
 
- Optimized the code for better performance and reliability.
- Implemented best practices to enhance maintainability and scalability.

----

# Progress Report - Daniel (4/4)

![height:600px](../Images/db1.jpg)

----

# Progress Report - Dylan-Matthew Garza

## Embedded Linux

- Deploying Microcontroller Firmware
    - Script to load using `remoteproc`

## Rust Server
- Loads Microcontroller firmware
- Reading and writing to Microcontroller
    - When IPC bridge is initiated `/dev/ttyRPMSG` file(s) appear
    - Virtual device file that can be read and written to ALMOST like a normal file

## Web Assembly Application
- Added Check box to use String Potentiometer
    - Updates Struct thats sent as `JSON` to Server

## Cortex-M4 Programming
- Using OpenAMP framework to communicate to Linux
    - Works by utilizing HAL drivers for UART
    - Wrote simple test program that expects messages and responds accordingly


----

# Embedded Linux with Yocto Project (1/2)

- Using Yocto Project
    - Combines the tools of OpenEmbedded and Bitbake
    - Build custom images 
- Custom `layer` for this project `meta-zf-project`
    - This `layer` describes everything about the image
        - All files on rootfs
        - All executable binaries
        - All system configuration

----

# Embedded Linux with Yocto Project (2/2)

<img src="../Images/yocto1.png" width="500">



----
# Rust Programming Language

- Object-Oriented
- Dynammically/Weakly Typed
- Interpreted 
- Similar to Java/Python
- Good for rapid development 

---- 

# Rust Programming Language

- Compiled Systems Language (like C/C++)
- Speeds that of or similar to C
- Type, thread, and memory safe language (memory leaks are near impossible)
    - No manual memory management OR garbage collection
    - Uses borrow checker and enforces rules on memory lifetimes during compilation
- Zero Cost Abastractions - no runtime cost of high-level features

![height:400px](../Images/rewrite-rust.png)

----

# Rust Server (1/2)

<div class="columns">
<div>
    <img src="../Images/rs-server1.png" width="600">
</div>
<div>
    <img src="../Images/rs-server3.png" height="200">
    <img src="../Images/rs-server2.png" height="200">
</div>
</div>

----

# Rust Server (2/2)

![height:600px](../Images/rs-server4.png)

----

# IPC with OpenAMP on console

![height:600px](../Images/console.png)

----

# Web Assembly Application (1/2)

<div class="columns">
<div>
    <img src="../Images/wasm1.png" height="300">
</div>
<div>
<img src="../Images/wasm2.png" height="400">
</div>
</div>

----

# Web Assembly Application (2/2)
![height:500px](../Images/wasm-app1.png)

----






