# SAP

SAP - Simple Assembly Project

This repository simulates a PDP-11 assembly environment written in Swift 3. 

Prerequisites:
  A Unix-like (Mac or Linux) system with Swift 3.x installed. With minimal testing, it seems to work under Swift 4, but it was written originally for Swift 3. Some errors may occur under Swift 4.

Operation:
  Place all files in a folder. Run `swift build` within the directory to "assemble" (ha!) the code into a binary file called SAP. This file will be placed at `$pwd`/.build/debug/SAP - move it to the main directory alongside the downloaded Swift and assembly files. Assign SAP execution privileges (`chmod +x SAP`) and run SAP (`./SAP`). 

Some basic assembly programs are included (Divide.txt, Factorial.txt) along with a 5-tuple turing machine simulator (TM3.txt). It takes instructions (tuples) in the form R(current state, symbol read, symbol written, direction, next state). The included set of tuples is a simple binary inverter.
