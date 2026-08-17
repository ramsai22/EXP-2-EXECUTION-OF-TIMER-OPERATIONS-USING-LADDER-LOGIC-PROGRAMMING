
# EXECUTION-OF-TIMER-OPERATIONS-USING-LADDER-LOGIC-PROGRAMMING


 #### NAME : PAIDA RAM SAI
 #### REGISTER NUMBER : 212223110034
 #### DEPARTMENT : CSE(IoT)
 #### YEAR : IV
 #### DATE : 27/07/2026

 
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

<img width="1496" height="525" alt="Screenshot 2026-07-27 150436" src="https://github.com/user-attachments/assets/a0d3665c-71f8-4792-af45-8761dd8c46a1" />
<img width="687" height="385" alt="Screenshot 2026-07-27 150505" src="https://github.com/user-attachments/assets/89ca5824-6b71-4280-bb93-69c3fb79b178" />
<img width="685" height="402" alt="Screenshot 2026-07-27 150514" src="https://github.com/user-attachments/assets/a5284021-b5b2-4cd6-a245-a19b536cfde3" />
<img width="793" height="522" alt="Screenshot 2026-07-27 150527" src="https://github.com/user-attachments/assets/72bd03b9-e909-4e7e-89de-ae5311e2b3cb" />
<img width="658" height="407" alt="Screenshot 2026-07-27 150535" src="https://github.com/user-attachments/assets/f19b83da-2970-4838-afc4-9c153b7c3bea" />
<img width="662" height="400" alt="Screenshot 2026-07-27 150553" src="https://github.com/user-attachments/assets/6eea2b80-ed68-4007-8a09-fec76285d5c7" />
<img width="695" height="387" alt="Screenshot 2026-07-27 150604" src="https://github.com/user-attachments/assets/4104b0ba-aded-4064-9525-439236e1c5f2" />
<img width="791" height="547" alt="Screenshot 2026-07-27 150615" src="https://github.com/user-attachments/assets/9f1713b3-8583-4220-b40a-ca3b42b98dc7" />

<img width="1915" height="983" alt="Screenshot 2026-07-27 150124" src="https://github.com/user-attachments/assets/b5021431-f1a6-4f2c-a070-12393127abb8" />

# Results:
The ladder logic programs for ON-delay, OFF-delay, and Retentive timers were successfully implemented and tested.
The observed outputs matched the expected behavior of each type of timer, demonstrating the correct functioning of timer operations in PLC ladder logic.
The experiment confirms the practical application of timers in controlling process sequences and managing time-dependent operations in industrial automation.
