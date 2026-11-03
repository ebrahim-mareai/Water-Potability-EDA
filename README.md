# Water Potability Exploratory Data Analysis

A Python data analysis project exploring water quality measurements and their relationship with potability labels. The notebook uses Pandas, NumPy, Matplotlib, and Seaborn to inspect the dataset, handle missing values for selected visualizations, and compare potable and non-potable water samples.

## Analysis Workflow

### Goal 1: Dataset Inspection & Missing-Value Handling

- **Data Loading**: Import water quality records from `water_potability.csv`.
- **Initial Inspection**: Display dataset dimensions and preview the first ten records.
- **Feature Review**: Examine nine water quality measurements alongside the `Potability` label.
- **Missing Values**: Apply median imputation to selected plotting series and analysis copies.
- **Before-and-After Visualization**: Plot selected measurements before and after filling missing values.

### Goal 2: Water Quality Visualization

- **Sample-Level Plots**: Visualize selected features across the first 200 samples using line, area, and scatter plots.
- **Feature Distributions**: Use histograms to examine the frequency distribution of water quality measurements.
- **Density Comparisons**: Compare feature distributions between potable and non-potable samples using density plots.
- **Pairwise Relationships**: Use a pair plot to explore relationships between features, with samples colored by potability.

### Goal 3: Potability Comparisons & Correlation Analysis

- **Feature Comparisons**: Plot each water quality measurement against the potability label.
- **Group Averages**: Compare average chloramine levels between potability categories.
- **Correlation Matrix**: Calculate Pearson correlations and display the results in an annotated heatmap.
- **Class Distribution**: Show the number and percentage of potable and non-potable samples in a bar chart.

## Dataset Features

| Feature | Description |
|---|---|
| `ph` | Acidity or alkalinity of the water |
| `Hardness` | Measurement associated with dissolved minerals such as calcium and magnesium |
| `Solids` | Total dissolved solids |
| `Chloramines` | Chloramine concentration |
| `Sulfate` | Sulfate concentration |
| `Conductivity` | Ability of the water to conduct electricity |
| `Organic_carbon` | Organic carbon concentration |
| `Trihalomethanes` | Trihalomethane concentration |
| `Turbidity` | Cloudiness of the water |
| `Potability` | Dataset classification: `0` for non-potable and `1` for potable |

## Tech Stack

- **Language**: Python 3
- **Data Handling**: `pandas`
- **Numerical Operations**: `numpy`
- **Visualization**: `matplotlib` and `seaborn`
- **Notebook Environment**: Jupyter Notebook / JupyterLab

## Project Files

- `WaterPotability_EDA.ipynb` — Data inspection, visualizations, comparisons, and analysis notes.
- `water_potability.csv` — Input dataset required to run the notebook; place it in the same directory as the notebook.

## Running the Notebook

1. Download the notebook and obtain `water_potability.csv`.
2. Place both files in the same directory.
3. Install the required packages:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyterlab
   ```

4. Launch JupyterLab:

   ```bash
   jupyter lab
   ```

5. Open `WaterPotability_EDA.ipynb` and run the cells in order.

## Analysis Observations

- The density and scatter plots show substantial overlap between the two potability categories across individual features.
- The correlation heatmap shows weak linear associations between individual water quality measurements and the potability label.
- The final bar chart summarizes the class distribution using sample counts and percentages.

These observations describe patterns in the dataset. Weak Pearson correlations do not rule out nonlinear relationships or interactions between features.

## Current Scope

This repository contains an exploratory analysis notebook. It does not include a trained prediction model or a deployed application. The plots use the potability labels supplied with the dataset; the analysis does not independently verify drinking-water safety.
