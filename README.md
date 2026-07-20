# Aspen Plus Flash Drum Automation with Python

## Overview

This project automates Aspen Plus simulations using Python and COM automation to analyze the vapor-liquid equilibrium of an ethanol-water flash separation process.

Python modifies the operating conditions of the flash drum, runs Aspen Plus automatically, extracts simulation results, and generates visualizations to identify how temperature and pressure affect ethanol separation.

This project demonstrates the integration of process simulation with Python for automated process analysis and data visualization.

---

## Features

- Automated Aspen Plus simulation control using Python
- Temperature and pressure parameter sweep
- Automatic extraction of simulation results
- Export of simulation data to a pandas DataFrame
- Heatmap visualization of ethanol vapor fraction
- Line plots showing the effect of temperature at different pressures

---

## Technologies Used

- Python 3
- Aspen Plus V14
- pywin32
- pandas
- NumPy
- Matplotlib

---

## Methodology

1. Create an ethanol-water flash drum simulation in Aspen Plus.
2. Connect Python to Aspen Plus using COM automation.
3. Vary flash temperature and pressure over a specified operating range.
4. Run the simulation for each operating condition.
5. Extract:
   - Vapor ethanol mole fraction
   - Vapor flow rate
   - Liquid ethanol mole fraction
   - Liquid flow rate
6. Store the results in a pandas DataFrame.
7. Generate visualizations to analyze separation performance.

---

## Example Results

The project generates:

- Heatmap of ethanol vapor fraction as a function of temperature and pressure.
- Temperature vs. ethanol vapor fraction curves for different pressures.
- Temperature vs. ethanol vapor flow curves for different pressures.

These visualizations help identify operating conditions that maximize ethanol concentration in the vapor phase.

---

## Running the Project

1. Ensure Aspen Plus V14 is installed.
2. Install the required packages:

```
pip install -r requirements.txt
```

3. Run the script:

```
python flash_simulation.py
```

The script will:

- Open the Aspen Plus model.
- Perform the temperature and pressure sweep.
- Extract vapor and liquid ethanol compositions.
- Generate plots showing the simulation results.

---

## Learning Outcomes

This project demonstrates:

- Aspen Plus process simulation
- Python automation using COM objects
- Data processing with pandas
- Scientific visualization with Matplotlib
- Process optimization through parameter studies

