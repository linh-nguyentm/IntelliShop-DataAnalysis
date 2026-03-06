# IntelliShop Pilot Study – Data Analysis

This repository contains the data analysis materials for the IntelliShop pilot study.

It is separated from the Unity project repository in order to keep the analytical workflow organized and to avoid mixing experimental application files with statistical analysis files.

## Repository Contents

The repository includes:

- `merged_data.csv`  
  The final merged dataset used for statistical analysis.

- `IntelliShop_DataAnalysis.ipynb`  
  Jupyter Notebook containing the data analysis workflow, including data preparation steps, descriptive statistics, and visualizations.

## Data Overview

The original study data consisted of multiple sources:

1. **Raw VR behavioral data**  
   Exported from the Meta Quest 3 headset, including participant session data such as trial number, product name, selected frame, reaction time, and deal value rating.

2. **Raw survey data**  
   Exported from the survey platform, including demographics, manipulation checks, smart shopper scale items, and additional attitudinal measures.

3. **Cleaned survey data**  
   A processed version of the survey data with incomplete responses removed, failed attention checks excluded, Likert scales recoded, and variable names standardized.

4. **Merged dataset**  
   The final dataset was created by merging the cleaned survey data with VR behavioral data using participant ID.

## Shared Data and Privacy

To protect participant privacy, this repository only includes:

- `merged_data.csv`

The raw VR files, raw survey responses, and intermediate cleaned survey files are **not shared in this repository**, as they may contain personal or potentially identifiable participant information.

This repository is therefore intended to provide only the analysis-ready dataset required to reproduce the reported results, while following data minimization and privacy protection principles.

## Purpose of `merged_data.csv`

`merged_data.csv` serves as the final dataset used for the statistical analysis in this project. It combines:

- cleaned survey responses
- behavioral VR data

This file is the only dataset required to run the analysis notebook included in this repository.

## Reproducibility

All results reported in the analysis were generated from `merged_data.csv` using:

- `IntelliShop_DataAnalysis.ipynb`

## Note

This repository contains only the data analysis component of the IntelliShop pilot study.

The Unity project, experimental application, and other implementation-related files are maintained in a separate repository.
