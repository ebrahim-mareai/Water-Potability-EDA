# Water Potability Exploratory Data Analysis

A Python data analysis project exploring water quality measurements and their relationship with potability labels.

## Analysis Workflow

### Goal 1: Dataset Inspection & Missing-Value Handling

- **Data Loading**: Import water quality records from `water_potability.csv`.
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

## Project Files

- `WaterPotability_EDA.ipynb`:  Data inspection, visualizations, comparisons, and analysis notes.
- `water_potability.csv`: Source [Kaggle Water Potability Dataset](https://www.kaggle.com/datasets/devanshibavaria/water-potability-dataset-with-10-parameteres)
