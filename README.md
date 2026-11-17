# EXECUTION-OF-TIMER-OPERATIONS-USING-LADDER-LOGIC-PROGRAMMING


 #### NAME : THARUN P S
 #### REGISTER NUMBER : 212224110055
 #### DEPARTMENT : BE.CSE(IOT)
 #### YEAR : 3

 
# Aim:
To understand and implement timer operations in a PLC using ladder logic and verify the output for different types of timers (ON-delay, OFF-delay, and Retentive timers).

# Apparatus Required:
Programmable Logic Controller (PLC) - A PLC that supports timer functions.
PLC Programming Software - Software such as RSLogix, TIA Portal, or CX-Programmer.
Computer System - For programming and simulating the PLC ladder logic.
Input Devices - Push buttons or switches for triggering the timer operations.
Output Devices - LEDs or any other indicators to visualize the timer output.
Wires and Connectors - For interfacing input/output devices with the PLC.
Power Supply - Appropriate power supply for the PLC and peripherals.
# Theory:
Timers in PLCs are used to introduce delays in control processes. They are fundamental in operations where the timing of events is crucial, 
such as starting a motor after a delay, turning off a light after a specified time, or maintaining a state for a fixed duration.

# Types of Timers:
 1. ON-Delay Timer (TON)
Functionality:

The ON-delay timer starts timing when the input condition becomes TRUE (ON).
After the preset time has elapsed, the timer output becomes TRUE (ON).
If the input condition turns FALSE (OFF) before the timer completes, the timer resets, and the output remains FALSE.
2. OFF-Delay Timer (TOF)
Functionality:

The OFF-delay timer starts timing when the input condition turns FALSE (OFF).
The timer output remains TRUE (ON) during the preset delay time and then turns FALSE (OFF) after the time has elapsed.
If the input condition becomes TRUE (ON) during the timing process, the timer resets.
3. Retentive ON-Delay Timer (RTO)
Functionality:

The Retentive ON-delay timer accumulates time as long as the input condition is TRUE (ON).
The accumulated time is retained even if the input condition turns FALSE (OFF).
The timer continues from the accumulated time when the input condition becomes TRUE again.
A separate reset input is usually provided to clear the accumulated time.
4. Pulse Timer (TP or TONR)
Functionality:

The Pulse Timer generates an output pulse of a specific duration when the input condition becomes TRUE (ON).
The output remains TRUE for the preset duration, regardless of the input state.
5. Timer-On Interval (TONI)
Functionality:

The Timer-On Interval is a variation of the ON-delay timer but is used to measure the time interval while the input is TRUE (ON).
The timer counts up as long as the input is TRUE and resets when the input turns FALSE.

 
# Procedure:
Setup the PLC Programming Environment:

Connect the PLC to the computer and launch the PLC programming software.
Ensure all input and output devices are connected to the PLC’s I/O modules.
Create Ladder Logic for Timers:

Implement the ON-delay timer (TON) by creating a rung with an input (e.g., a push button) linked to a TON instruction. Set the preset time (e.g., 5 seconds).
Implement the OFF-delay timer (TOF) by creating a rung with an input linked to a TOF instruction. Set the preset time (e.g., 5 seconds).
Implement the Retentive Timer (RTO) by creating a rung with an input linked to an RTO instruction. Set the preset time and enable an additional rung to reset the timer when required.
Simulate the Ladder Logic:

Run the simulation in the PLC software.
Test the ON-delay timer by pressing the input button and observing the delay before the output is activated.
Test the OFF-delay timer by deactivating the input and observing the delay before the output turns off.
Test the Retentive Timer by toggling the input on and off, observing how the accumulated time is retained.
Download and Execute:

Download the ladder logic program to the PLC if available and run it.
Test the timers with the physical push buttons and observe the LEDs or other output devices.
#   Outputs:
ON-Delay Timer: The output LED or indicator should turn on after a specified delay (e.g., 5 seconds) once the input is activated.
OFF-Delay Timer: The output should remain on for the specified delay after the input is deactivated, and then it should turn off.
Retentive Timer: The output should turn on after the accumulated time reaches the preset value, and it should retain the accumulated time even if the input is turned off.


# Simulation Screenshots 


<img width="1016" height="508" alt="Screenshot 2026-11-17 110323" src="https://github.com/user-attachments/assets/11e0b4da-3aac-4cb7-ba06-ac6196dc59f0" />

<img width="1016" height="514" alt="Screenshot 2026-11-17 110401" src="https://github.com/user-attachments/assets/e15ca85a-f232-43f3-b2d6-1f3f1d78c7dc" />

<img width="1012" height="648" alt="Screenshot 2026-11-17 110430" src="https://github.com/user-attachments/assets/bd36115f-e9d9-4229-a82d-205732a53d2a" />

<img width="1018" height="720" alt="Screenshot 2026-11-17 110511" src="https://github.com/user-attachments/assets/f5cec9fe-c10f-4f1a-813f-39618b66e349" />


# Results:
The ladder logic programs for ON-delay, OFF-delay, and Retentive timers were successfully implemented and tested.
The observed outputs matched the expected behavior of each type of timer, demonstrating the correct functioning of timer operations in PLC ladder logic.
The experiment confirms the practical application of timers in controlling process sequences and managing time-dependent operations in industrial automation.
