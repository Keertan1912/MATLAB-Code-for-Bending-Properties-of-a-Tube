# MATLAB-Code-for-Bending-Properties-of-a-Tube

## Overview
This MATLAB script calculates and plots the bending properties of a tube as a function of its inner diameter. The calculated properties include:
- **Bending Strength**
- **Bending Stiffness**
- **Bending Energy**

The results are displayed in the command window and plotted graphically.

## Code Functionality
1. **Initialization**: The script initializes empty arrays for bending properties and defines a loop variable `c`.
2. **Computation**: Using a while loop, it iterates over different values of inner diameter (`1.27 * c` in inches) to compute:
   - **Bending Strength** using the formula:
     \[ \frac{M \cdot C}{I} \]
   - **Bending Stiffness** using the formula:
     \[ \frac{M \cdot 1000}{3 \cdot 205 \cdot I} \]
   - **Bending Energy** using the formula:
     \[ \frac{(435^2) \cdot I \cdot 4 \cdot 64}{205 \cdot 25.4^2 \cdot \pi \cdot (1.27c)^2 \cdot 1000} \]
3. **Results Output**: The computed values are printed to the command window.
4. **Graph Plotting**: A plot is generated to visualize the relationship between inner diameter and the three bending properties.

## Plot Details
- **X-Axis**: Inner diameter (in inches)
- **Y-Axis**: Force applied per unit area (N/mm²)
- **Legend**:
  - **Bending Strength** (Blue `--b*`)
  - **Bending Stiffness** (Green `--g*`)
  - **Bending Energy** (Red `--r*`)

## Prerequisites
- MATLAB installed on your system.
- Basic understanding of MATLAB scripting.

## How to Run the Code
1. Open MATLAB.
2. Copy and paste the script into a new script file (e.g., `bending_properties.m`).
3. Run the script.
4. The output values will be displayed in the command window, and a plot will be generated.

## Notes
- The script runs for 19 iterations (`c = 1` to `c < 20`).
- Ensure that the formulas match the intended physics-based calculations.
- Modify `M`, `C`, or other parameters as needed for different scenarios.

## Author
This script is provided as-is. Feel free to modify and extend it as per your requirements.

