# Data Documentation – IntelliShop Pilot Study

## 1. Raw VR Data

The folder `/data/` contains the raw behavioral data exported directly from the Meta Quest 3 headset.  
Each CSV file corresponds to one participant session and includes:

- Participant ID  
- Trial number  
- Product name  
- Selected frame (discount vs. points)  
- Reaction time (milliseconds)  
- Deal value rating  

These files represent unprocessed runtime output from the Unity application.

---

## 2. Raw Survey Data

**File:**  
`Cash Now or Points Later? (Responses).xlsx`

This file contains the raw questionnaire responses collected after the VR task.  
It includes:

- Demographics  
- Manipulation check responses  
- Smart shopper scale  
- Additional attitudinal measures  

This file is exported directly from the survey platform and has not been cleaned.

---

## 3. Cleaned Survey Data

**File:**  
`survey_clean.csv`

This file contains:

- Removed incomplete responses  
- Removed failed attention checks  
- Recoded Likert scales  
- Standardized variable names  

This dataset is used for merging with VR behavioral data.

---

## 4. Merged Dataset

**File:**  
`merged_data.csv`

This dataset merges:

- Cleaned survey responses (`survey_clean.csv`)  
- Behavioral VR data (from `/data/`)

Merging is conducted using the participant ID as the key.

This file serves as the final dataset used for statistical analysis.

---

## 5. Data Analysis Code

**File:**  
`Group_1_Data_Analysis_Final.ipynb`

This Jupyter notebook contains:

- Data cleaning procedures  
- Descriptive statistics  
- Visualization  

All results reported in the paper are generated from `merged_data.csv` using this script.
