# Vex-V5-Simulink-Expansion

## About The Project
This library incorporates the MATLAB-provided [VEX EDR V5 Robot Brain Support from Simulink](https://uk.mathworks.com/hardware-support/vex-edr-v5.html) into a higher level interface, alongside some addition functionality for the [VEX V5 Workcell](https://www.vexrobotics.com/v5/products/workcell) kit.

## Getting Started

### Prerequisites
- The official [VEX EDR V5 Robot Brain Support from Simulink](https://uk.mathworks.com/hardware-support/vex-edr-v5.html) library.
- The [Advanced Smart Motor Blocks](https://uk.mathworks.com/matlabcentral/answers/435564-vex-v5-motor-voltage) files to be in the workspace directory. The files are provided in this repository for convenience, though were originqlly published in MATLAB answers as linked.

### Installation
After downloading, ensure the `Vex-V5-Simulink-Expansion.slx`, `Advanced_SmartMotorRead.m` and `Advanced_SmartMotorWrite.m` are in the same working directory as the model the library is to be used in. Once this is completed, the library should appear in the Simulink Library Browser.

## Important Information
- The 'Inverse Kinematic Calculation' and 'Inverse Kinematic Motion' blocks make no checks to ensure the output position can be reached. These limits must be included in your model.
- The Vex V5 Arm home position in the 'Angle to Potentiometer' and 'Potentiometer to Angle' is defined by the joint angles in the block MATLAB code. These can be changed to suit the home jig that is being used.

## License
Distributed under the MIT License. See `LICENSE.txt` for more information.
