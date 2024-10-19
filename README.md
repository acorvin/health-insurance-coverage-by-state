
# US Health Insurance Coverage by State (2016) - Interactive Data Visualization

This project visualizes the 2016 Health Insurance Coverage data for each US state using an interactive map powered by Plotly's `scatter_mapbox`. The visualization highlights differences in health insurance coverage across states, with Medicaid and Medicare enrollment figures available in the tooltip on hover.

## Preview
![Interactive Map](interactive-map.gif)


## Table of Contents
- [Overview](#overview)
- [Project Setup](#project-setup)
- [Data](#data)
- [Features](#features)
- [Usage](#usage)
- [Customization](#customization)
- [Dependencies](#dependencies)
- [Data Sources](#data-sources)
- [License](#license)

## Overview
This project uses health insurance coverage data from 2016 to create an interactive map where users can explore various enrollment statistics by state. The size and color of the markers on the map represent the total health insurance coverage in each state, with additional details (Medicaid and Medicare enrollment) available when hovering over each state.

### Features:
- Interactive map visualization with Plotly
- Hover tooltips displaying state-specific information (Health Insurance, Medicaid, and Medicare enrollments)
- Color-coded and sized markers based on health insurance coverage
- Custom styling of tooltips

## Project Setup

To set up this project on your local machine, follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/acorvin/health-insurance-coverage.git
cd health-insurance-coverage
```

### 2. Install Dependencies
Ensure you have Python 3.x and Jupyter Notebook installed. Then install the required Python packages:

```bash
pip install pandas plotly jupyter
```

### 3. Data Preparation
Place your data file (`health_insurance_coverage_by_state_2016.csv`) in the `data/` folder. Ensure your CSV file has the following columns:
- `state`: The state name.
- `latitude`: The latitude for the state's center.
- `longitude`: The longitude for the state's center.
- `health_insurance_coverage`: The total health insurance coverage for the state.
- `medicaid_enrollment`: The Medicaid enrollment for the state.
- `medicare_enrollment`: The Medicare enrollment for the state.

Example CSV file structure:

```csv
state,latitude,longitude,health_insurance_coverage,medicaid_enrollment,medicare_enrollment
Alabama,32.806671,-86.79113,4800000,1100000,800000
Alaska,61.370716,-152.404419,720000,150000,120000
...
```

## Usage

Once the setup is complete, launch the Jupyter Notebook:

```bash
jupyter notebook
```

Open the analysis.ipynb file in the Jupyter interface. You can run all cells to generate the interactive map within the notebook.

## Customization

- You can modify the color scale by changing `color_continuous_scale` to another Plotly color scale such as `Plasma`, `Cividis`, or `Turbo`.
- To adjust zoom levels, modify the `zoom` argument.
- Change the hover template to show different data or format it differently by editing the `hovertemplate` section in the code.

## Dependencies

- `pandas`: For data manipulation.
- `plotly`: For creating interactive maps.
- `jupyter`: To run the notebook.

Install them via `pip`:

```bash
pip install pandas plotly jupyter
```

## Data Sources
[Health Insurance Coverage](https://www.kaggle.com/datasets/hhs/health-insurance)

## License

This project is licensed under the [MIT license](https://opensource.org/licenses/MIT).
