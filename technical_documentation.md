# Technical Documentation: World Happiness Data Analysis

## Project Description
This project conducts an Exploratory Data Analysis (EDA) on the World Happiness Report, a study that measures and ranks happiness across 156 countries. The goal is to identify which factors are most important for living a happier life, enabling countries and individuals to focus on the most significant factors.

## Project Structure
```
happiness-eda-project/
├── data/
│   ├── raw/              # Original unprocessed data
│   │   └── happiness_score.csv
│   └── processed/        # Processed data
│       └── descriptive_stats.csv
├── images/               # General project images
├── notebooks/           # Jupyter notebooks
│   └── happiness_eda.ipynb
├── presentation/        # Presentation files
├── reports/            # Generated reports
├── utils/             # Utility functions
│   └── functions_EDA.py
└── visualizations/    # Generated graphics
    └── univariate_plots/
        ├── dist_freedom_to_make_life_choices.png
        ├── dist_gdp_per_capita.png
        ├── dist_generosity.png
        ├── dist_overall_rank.png
        ├── dist_perceptions_of_corruption.png
        ├── dist_score.png
        ├── dist_social_support.png
        └── dist_year.png
```

## Dataset
The main dataset (`happiness_score.csv`) contains the following variables:
- **Overall rank**: Happiness ranking of different countries
- **Country or region**: Country or region name
- **Score**: National average of responses (scale 0-10)
- **GDP per capita**: Gross Domestic Product per capita
- **Social support**: Level of social support (scale 0-2)
- **Freedom to make life choices**: Freedom of choice (scale 0-1)
- **Generosity**: Level of generosity (scale 0-1)
- **Perceptions of corruption**: Corruption perception (scale 0-1)
- **Year**: Year of study

## Dependencies
The project requires the following Python libraries:
- pandas: Data manipulation and analysis
- numpy: Numerical computing
- seaborn: Statistical visualization
- matplotlib: Graphics creation

Installation:
```bash
pip install -r requirements.txt
```

## Analysis Process
1. **Data Loading and Cleaning**
   - Column name standardization
   - Null value handling
   - Duplicate checking
   - Data range validation

2. **Exploratory Analysis**
   - Descriptive statistics
   - Univariate analysis
   - Key variable distributions
   - Pattern and trend identification

3. **Visualization**
   - Distribution plots for each variable
   - Visualization storage in PNG format
   - High resolution (300 dpi) for presentation use

## Results and Artifacts
- **Descriptive Statistics**: Stored in `data/processed/descriptive_stats.csv`
- **Visualizations**: Available in `visualizations/univariate_plots/`
- **Main Notebook**: `notebooks/happiness_eda.ipynb` contains all analysis with detailed comments

## Version Control
This project is version controlled with Git and hosted on GitHub under the MIT license.

## Author
- Ana Gamito
