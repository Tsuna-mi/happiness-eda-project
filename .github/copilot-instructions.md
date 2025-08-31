# AI Agent Instructions for Happiness EDA Project

## Project Overview
This is a data analysis project focusing on the World Happiness Report. The project follows a structured data science workflow with clear separation of data, analysis, and visualization components.

## Key Components and Data Flow

### Data Pipeline
1. Raw data (`data/raw/happiness_score.csv`)
   - Source: World Happiness Report
   - Contains happiness metrics across countries and years
   - Key metrics: GDP, social support, freedom, corruption perception

2. Processing
   - Processed data stored in `data/processed/`
   - Key output: `descriptive_stats.csv` for statistical summaries

3. Visualizations
   - Generated plots stored in `visualizations/univariate_plots/`
   - Standard naming convention: `dist_{variable_name}.png`

## Project Structure Conventions

### Directory Organization
```
happiness-eda-project/
├── data/              # Data segregation pattern
│   ├── raw/          # Immutable original data
│   └── processed/    # Transformed/analyzed data
├── notebooks/        # Analysis notebooks
├── utils/           # Reusable functions
└── visualizations/  # Generated plots
```

### Coding Patterns

1. Data Analysis Functions
- Location: `utils/functions_EDA.py`
- Common operations for data cleaning and transformation
- Example usage found in `notebooks/happiness_eda.ipynb`

2. Notebook Structure
- Follow the established flow:
  1. Data loading and inspection
  2. Cleaning and standardization
  3. Analysis and visualization
  4. Results export

## Key Workflows

### Setting Up Development Environment
```bash
pip install -r requirements.txt
```

### Data Analysis Process
1. Main analysis notebook: `notebooks/happiness_eda.ipynb`
2. Functions from `utils/functions_EDA.py` for common operations
3. Export results to `data/processed/`
4. Save visualizations to `visualizations/univariate_plots/`

## Project-Specific Conventions

### Visualization Standards
- Distribution plots saved as PNG with 300 dpi
- Standard naming pattern for clarity
- Plots stored in dedicated subdirectories by type

### Data Processing
- Column names standardized to snake_case
- Missing values handled explicitly
- Data validation checks for value ranges

## Documentation Links
- Technical details: [technical_documentation.md](../technical_documentation.md)
- Project overview: [README.md](../README.md)

## Best Practices
1. Always use relative paths from notebooks
2. Document analysis steps and insights
3. Save processed data and visualizations in appropriate directories
4. Follow established naming conventions for files and variables
