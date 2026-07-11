# Telco Customer Churn Prediction & EDA

This project performs an Automated Exploratory Data Analysis (EDA) and visualization pipeline on telecom customer churn data. It uses a clean, reproducible project-local environment managed by `renv`.

## 📦 Project Structure

```text
customer-churn-prediction/
├── data/
│   └── raw/
│       └── Telco-Customer-Churn.csv  # Raw dataset (Git-ignored)
├── renv/                             # Local project environment infrastructure
├── .gitignore                        # Files excluded from GitHub tracking
├── .Rprofile                         # Auto-activates renv when project opens
├── renv.lock                         # Exact package version blueprint
├── run_analysis.R                    # Complete analysis script
└── README.md                         # Project documentation
```

## 🚀 Getting Started

Follow these steps to replicate the environment and run the analysis on your machine.

### 1. Prerequisites
Ensure you have [R](https://r-project.org) installed (built on version 4.6.1).

### 2. Clone the Repository
```bash
git clone https://github.com/rchinmay91/customer-churn-prediction.git
cd customer-churn-prediction
```

### 3. Add the Dataset
Because the raw data is large, it is omitted from this repository. 
1. Download `Telco-Customer-Churn.csv`.
2. Create a folder structure: `data/raw/` inside the root directory.
3. Place the CSV file directly into `data/raw/`.

### 4. Restore the Environment & Run
Open your R console or RStudio inside the project directory. `renv` will automatically bootstrap itself. Run the following to install all exact package dependencies:

```R
# Restore project-specific packages (tidyverse, DataExplorer, etc.)
renv::restore()

# Run the complete analysis pipeline
source("run_analysis.R")
```

## 📊 Outputs Generated

* **`churn_eda_report.html`**: An interactive, comprehensive HTML profiling report profiling missing values, distributions, and feature correlations.
* **Churn Visualization**: A proportional bar chart displayed in your R graphics device showing Churn Rate segmented by Contract Type.

## 🛠️ Built With

* [R 4.6.1](https://r-project.org) - Statistical computing language.
* [tidyverse](https://tidyverse.org) - For data manipulation and visualization.
* [DataExplorer](https://github.io) - For automated data exploration.
* [renv](https://github.io) - Dependency management engine.
