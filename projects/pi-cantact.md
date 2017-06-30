---
layout: project
type: project
image: images/cantact1.jpg
title: Pi-CANtact
permalink: projects/pi-cantact
date: 2017
labels:
  - OBD
  - CANtact
  - Pyvit
  - Python
summary: Scripts to interface with CAN bus devices such as OBD using CANtact and Pyvit on a Raspberry Pi.
---
### Project Overview
Pi-CANtact is a collection of scripts used to interface with on-board diagnostics (OBD) using the CANtact protocol to extract data packets. OBD refers to a vehicle's self-diagnostic and report capability as this protocol uses standardized digital communication ports to provide real-time data. In addition, this protocol provides a standardized series of diagnostic trouble codes which allow one to rapidly identify and remedy malfunctions within the vehicle. Pi-CANtact is the software module used to extract OBD data, which is then fed into a block chain module to ensure secure car-to-car communications. The Python scripts utilize the [Pyvit](https://github.com/linklayer/pyvit) toolkit which implements common hardware interfaces and protocols used in the automotive systems. In addition to Pyvit, [python-OBD](https://github.com/brendan-w/python-OBD) is used for handling real-time sensors data from OBD-II vehicle ports. 

### Script Development
The module was incrementally built by creating scripts to display messages on the bus in real time. These messages were decoded as the frame ID and packet data could be extracted. Various versions were implemented which included options for ID, decimal, and hexadecimal filtering. After implementing packet decoding and extraction, scripts to send CAN frames onto the bus were written which included sending arbitrary interface identifiers and data bytes. Finally, scripts were written to request sensor queries according to OBD command tables where specific values such as intake air temperature, engine RPM, or fuel pressure could be requested. 

### Learning Outcomes
From this project, I learned both technical and project management skills. On the technical side, I learned how to use various APIs from the OBD and Pyvit libraries, gained more experience working with Python, learned how to interface with the CAN protocol, and became familiar with the Raspberry Pi serial interface. I also strengthened my skills involving Git for version control. Regarding project management, I learned how to effectively break down tasks within a module into smaller incremental steps. 

Source: <a href="https://github.com/nathancy/Pi-CANtact"><i class="large github icon"></i>https://github.com/nathancy/Pi-CANtact</a>
