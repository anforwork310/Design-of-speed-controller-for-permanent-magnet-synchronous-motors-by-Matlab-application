# Design of speed controller for permanent magnet synchronous motors by Matlab application
Simulation on Matlab application

## I. Introduction
  Permanent magnet synchronous motors are widely used in mid and low applications. The growth of permanent magnet motor (PM) drives in the market  has demanded the need of simulation tools capable of handling motor drive simulations. In this project, the simulation of a field oriented controlled PM motor drive system is developed using Simulink. Simulink in Matlab application have helped the process of developing systems including the capabilities of performing dynamic simulations of motor drives.

## II. Operation Principle
<img width="1066" height="605" alt="image" src="https://github.com/user-attachments/assets/f5d3dcb7-1177-4383-8ac8-7516fb0c84dc" />

- The goal of the FOC on synchronous machine is to be able to separately control the torque producing and magnetizing flux components. FOC control will allow us to decouple the torque and the magnetizing flux components of stator current. 
- With decoupled control of the magnetization, the torque producing component of the stator flux can now be thought of as independent torque control. To do the above steps, we will use Clarke and Park transformations. Clarke and Park transformations are mainly used in vector control architectures related to permanent magnet synchronous machines. 

## III. Paradigm
<img width="1387" height="746" alt="image" src="https://github.com/user-attachments/assets/822c6e53-9d29-498f-973b-d57d5e96d73a" />

To perform a complete simulation, we perform the following steps:
- Step 1: Check the PMSM block algorithm, the PI Controller Block and Function Block in Simulink application.
- Step 2: We calculate the switching frequency based on the current frequency.
- Step 3: Then we calculate the factor 𝑘_𝑝 and 𝑘_𝑖 of the PI controller 
- Step 4: We control the PMSM to run at the desired speed at the input.
- Step 5: The desired signal is used to compare with the signal obtained.
- Step 6: We check the results obtained after simulation.

<img width="1408" height="539" alt="image" src="https://github.com/user-attachments/assets/d35768cc-08fc-43b6-bcda-5bb4d2bc14db" />

Through examining the working quality of the system in typical cases, we see that the system operates stably. However, the current at start-up remains high but then returns to steady state at steady state. Motor torque meets the load value we put in. But this is the result based on ideal condition, I will use the output signal after going through PI controller and I will connect to PMSM directly. To get more accurate results, we need to experiment more in practice to get more consistent results.

## VI. Conclusion
- Learn about electric vehicles and the engines used for electric vehicles
- Building a mathematical model of the PMSM.
- Build simulation model of PMSM engine using Matlab/Simulink
- Build a PI controller for PMSM
- Surveying the working quality of the system in typical cases.




