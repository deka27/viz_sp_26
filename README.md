# Kickstarter Network Visualization

This project analyzes Kickstarter project data and builds three network-based visualizations from a single notebook.

## Project Contents

- `viz.ipynb`: main analysis notebook with markdown narrative and chart generation.
- `Kickstarter Projects_639378_Aug 2025 Updated.csv`: source dataset used by the notebook.
- `category_network.png`: category similarity network output.
- `country_category_bipartite_clean.png`: country-to-category bipartite network output.
- `creator_movement_network.png`: creator movement network output.

## Notebook Structure (`viz.ipynb`)

1. Data loading and feature engineering.
2. Graph 1: category similarity network.
3. Graph 2: country-to-category specialization (bipartite) network.
4. Graph 3: creator movement across categories.

All imports are grouped at the top of the notebook for easier maintenance.

## Requirements

- Python 3.10+
- `pandas`
- `numpy`
- `networkx`
- `matplotlib`
- `seaborn`
- Jupyter (`notebook` or `jupyterlab`)

## Run

1. Install dependencies:
   ```bash
   pip install pandas numpy networkx matplotlib seaborn jupyterlab
   ```
2. Start Jupyter:
   ```bash
   jupyter lab
   ```
3. Open `viz.ipynb` and run cells top-to-bottom.

## Dataset Download

- Kaggle dataset page: [Kickstarter Dataset 629,147 Projects (May 2025)](https://www.kaggle.com/datasets/domingosun/kickstarter-dataset-629147-projects-may-2025?select=Kickstarter+Projects_May+2025+-+SAMPLE.csv)
- The Kaggle files shown directly are sample data.
- For the full ~629k-project file, open the dataset page and check the **About Dataset** section for the external link labeled `Kickstarter data (Dec 2025)`.
- That external full-data link may change over time, so use the label on the Kaggle page as the source of truth.

## Notes

- The notebook expects the CSV file to remain in the project root directory.
- Re-running the notebook will regenerate the three `.png` output files.
