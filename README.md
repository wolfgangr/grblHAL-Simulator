# closed loop PID pulse generation


Idea:  
- Attach a linear encoder to a the axes of a CNC machine
- feed back the signal to grblHAL
- replace deterministic Bresenham code generation by adaptive PID

expected benefits:
- no loss of steps
- automagically offset backlash and other drive chain imperfections
- push performance of stepper systems
- keep homing over all states
- allow automated restart after shutdown

Discussion and development log here:  
["Long closed loop" from linear encoder into grbl stepper for dynamic backlash compensation #563](https://github.com/grblHAL/core/discussions/563)

This fork is intended for developping the algorithm and code interface

[Original README.md of grblHAL Simulator](README_orig.md)


