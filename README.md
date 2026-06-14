# Healthcare_Analysis

# WASH Infrastructure Data Analysis Pipeline 🌍📊

## Project Overview
This repository features a Python-based data processing and visualization pipeline designed to analyze global Water, Sanitation, and Hygiene (WASH) metrics. Using time-series data from the WHO/UNICEF Joint Monitoring Programme (2000–2022), the project tracks key public health trends, performs data reshaping, and generates publication-ready visualizations to highlight the real-world impacts of targeted public policy interventions.

## Tech Stack
* **Language:** Python 3.x
* **Data Libraries:** `pandas`, `numpy`
* **Visualization:** `seaborn`, `matplotlib`

## Technical Workflow
1. **Data Cleaning:** Handles programmatic renaming and structures columns for tracking population shares across safely managed sanitation, drinking water, and basic hygiene metrics. Null values are filtered selectively per analysis to ensure data integrity.
2. **Spectrum Analysis:** Subsets and isolates distinct global entities (Developed, Emerging, and Developing baselines) to map comparative infrastructure scaling over a two-decade timeline.
3. **Dimensional Reshaping:** Utilizes `pandas.melt()` to convert "wide" metric datasets into a "long" format. This allows `seaborn` to map feature variables dynamically to the color (`hue`) parameters for clean categorical line plots.
4. **Data Storytelling & Visualization:** Renders high-resolution (300 DPI) line graphs complete with custom palettes, boundary limits, and chronological policy intervention markers.

## Key Insights Captured
* **The Infrastructure vs. Behavior Split:** Visualizes how behavioral metrics (e.g., access to basic handwashing facilities) can scale significantly faster than heavy capital-intensive structural grid deployments (e.g., sewage infrastructure), as evidenced in targeted country deep-dives following major national sanitation campaigns.
* **The Tracking Gap:** Exposes structural variance in global reporting, where highly developed benchmarks often phase out tracking foundational metrics once baseline saturation is achieved.

## Repository Assets
* `WASH_Analysis.ipynb` - Complete data transformation and visualization pipeline.
* `clean_water_and_sanitation.csv` - Ingested time-series source data.
* Output Visualizations (`.png`) - Generated high-resolution trend charts.
