# Flow Control Loop using PID and Model Predictive Control (MPC)

## Overview
This project focuses on the modelling, simulation, and real-time implementation
of a closed-loop flow control system using classical PID control and advanced
Model Predictive Control (MPC).

The objective is to analyse system performance, stability, and dynamic response
using control theory tools and to validate the results through real-time
hardware implementation.


## Objectives
- Model a flow control process using first-principle methods
- Analyse system stability and dynamic behaviour
- Design and tune P, PI, PD, and PID controllers
- Implement Model Predictive Control (MPC)
- Compare the performance of PID and MPC controllers


## System Architecture
**Control Flow:**  
Flow Transmitter → Arduino → Controller (PID / MPC) → I/P Converter → Control Valve → Process

The controller receives real-time flow measurements and computes the control
signal required to regulate the flow at the desired setpoint.


## Hardware Components
- Centrifugal Pump
- Pneumatic Control Valve
- I/P Converter (4–20 mA to 3–15 psi)
- Flow Transmitter (4–20 mA)
- Arduino (Data acquisition and control)
- Power supply, piping, and reservoir


## Software & Tools
- Arduino IDE
- MATLAB
- Simulink
- Control System Toolbox
- Model Predictive Control Toolbox


## Control Methodology

### Classical PID Control
- Transfer function derived from physical modelling
- PID parameters tuned using MATLAB tools
- System analysed using:
  - Step response
  - Root locus
  - Bode plot
  - Time-domain performance metrics


### Model Predictive Control (MPC)
Model Predictive Control uses an internal model of the process to predict future
system behaviour and optimise control actions over a finite horizon.

Advantages of MPC:
- Improved disturbance rejection
- Reduced overshoot
- Better handling of constraints
- Faster settling time compared to PID


## Results & Discussion
- PID control achieved stable flow regulation with acceptable transient response
- MPC showed superior performance in terms of overshoot reduction and robustness
- Simulation results closely matched real-time experimental behaviour


## Applications
- Industrial flow regulation systems
- Chemical and process industries
- Control system laboratories
- Academic and training environments


## Future Scope
- Adaptive and nonlinear MPC implementation
- IoT-based monitoring and control
- Integration with industrial communication protocols
- Multi-loop and cascade control systems


## License
This project is licensed under the MIT License.
