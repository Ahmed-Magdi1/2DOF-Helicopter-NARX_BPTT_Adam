# 2DOF-Helicopter-NARX_BPTT_Adam

## Overview
This project models the nonlinear dynamics of a 2-DOF helicopter system using a Nonlinear AutoRegressive model with eXogenous inputs (NARX) neural network. The model predicts the system's behavior based on lagged input-output features, leveraging temporal dependencies to output pitch and yaw angles.

## Colab Link
You can access the Google Colab notebook for this project: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gp0SwaDJU_nWepFkGd1MYBU1pv2_tfaQ?authuser=0#scrollTo=0llz0160HQs7)

## Data Used
The model is trained and validated using real sequential data representing the helicopter's behavior:
- **Input Variables**:
  - `V`: Voltage applied to the motors (constant for both motors).
  - `I_pitch`: Current for the pitch motor.
  - `I_yaw`: Current for the yaw motor.
- **Output Variables**:
  - `pitch_angle`: The pitch angle of the helicopter.
  - `yaw_angle`: The yaw angle of the helicopter.

### Data Format
The input and output data are stored in separate CSV files:
- [`inputs.csv`](inputs.csv): Contains columns `V`, `I_pitch`, `I_yaw`.
- [`outputs.csv`](outputs.csv): Contains columns `pitch_angle`, `yaw_angle`.
