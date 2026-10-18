# Group 4 — Data Cleaning and Exploratory Data Analysis
**Repository:** [iaac-maai/Group4-day1-assignment](https://github.com/iaac-maai/Group4-day1-assignment)

## Team Members
- Fawad
- Hetashri
- Daria
- Luis

## 1. Use case

This project investigates residential building energy performance and consumption using a built-environment dataset. The aim is to understand the dataset's quality, explore relationships between building characteristics and energy demand, and communicate evidence through descriptive statistics and visualizations. The exploratory analysis focuses on Energy Performance Certificates (EPC) and gas and electricity consumption, including historical trends where suitable data is available. The resulting cleaned dataset is intended to support future predictive modelling.

## 2. Project Overview

This project focuses on cleaning, preprocessing, and performing Exploratory Data Analysis (EDA) on property-level energy consumption data.

The analysis explores electricity and gas consumption patterns, Energy Performance Certificate (EPC) distributions, and differences in energy consumption across property types.

## 3. Dataset

**Dataset:** 

| Attribute | Description |
|---|---|
| Dataset name | National Energy Efficiency Data-Framework (NEED): anonymised data 2026 |
| Original source | [Department for Energy Security and Net Zero](https://www.gov.uk/government/organisations/department-for-energy-security-and-net-zero) |
| Geographic coverage | UK |
| Unit of observation | Property-level data containing gas and electricity consumption from 2005 to 2024, property characteristics, and energy-efficiency measure installations. |
| Raw size | 50,000 rows × 96 columns |
| Temporal coverage | 2005-2024 |
| Important fields | Insert exact EPC, gas, electricity and building-characteristic column names |

### 4. Local Dataset

The notebook reads the anonymised dataset from: data/anon2026_50k.csv

## 5. Research questions

1. How are EPC ratings distributed across the properties in the dataset, and how do they relate to energy use where comparable observations exist?
2. How has gas consumption changed over 2005–2024, **if annual data for that full period is available**?
3. How has electricity consumption changed over 2005–2024, **if annual data for that full period is available**?
4. What is the co-relation across different energy ureses over 2005-2024, **if annual data for that full period is available**?

## 6. Project Structure

```text
Group4-day1-assignment/
├── data/
│   ├── .gitkeep
│   └── anon2026_50k.csv
├── figures/
│   ├── average_energy_by_building_type.png
│   ├── epc_distribution.png
│   ├── average_annual_gas_consumption.png
│   ├── average_annual_electricity_consumption.png
│   └── gas_vs_electricity_consumption_trends.png
├── uk_energy_consumption_eda.ipynb
├── requirements.txt
├── .gitignore
└── README.md

## 5. How to run

Clone the repository and enter the project folder:

```bash
git clone https://github.com/iaac-maai/Group4-day1-assignment.git
cd Group4-day1-assignment
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on **Windows PowerShell**:

```powershell
.\.venv\Scripts\Activate.ps1
```

Or on **macOS/Linux**:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Open `notebook/data_cleaning_and_EDA.ipynb` in Jupyter in VS Code, select the `.venv` Python kernel, then choose **Restart Kernel → Run All**. The notebook should acquire or load its input data and create the cleaned dataset and exported figures using relative paths. **Confirm the actual download method and paths in the final notebook before publishing these instructions.**

## 6. Data quality checks and cleaning

The cleaning workflow checks for duplicated records, missing values, inconsistent data types and potential outliers. Each change should be documented in the notebook with a reason for the decision.

| Quality check | Observed result | Action / justification |
|---|---|---|
| Duplicate rows | [Insert actual number] | [Explain whether records were removed and why] |
| Missing values | [Insert affected columns and percentages] | [Explain whether values were retained, imputed or excluded] |
| Data types | [Insert any detected issues] | [Describe conversions, if any] |
| Outliers | [Insert variables inspected] | [Explain whether extreme values are plausible or erroneous] |
| Feature engineering | [Insert new variable, if created] | [Explain its built-environment relevance] |

**Cleaned output:** `[insert exact relative path and filename]`.

## 7. Exploratory data analysis

The notebook should contain descriptive statistics, univariate distributions, bivariate comparisons, grouped summaries and correlation analysis. Interpretations must distinguish observed associations from causal relationships.

### EPC distribution and energy performance

[Insert the observed EPC distribution, a numeric finding and its interpretation.]

![EPC distribution](figures/[replace-with-actual-epc-figure].png)

### Gas consumption trends

[Insert actual start/end values, units, trend description and coverage limitations. Clarify whether the values are totals, means or an index with 2005 = 100.]

![Gas consumption trend](figures/[replace-with-actual-gas-figure].png)

### Electricity consumption trends

[Insert actual start/end values, units, trend description and coverage limitations.]

![Electricity consumption trend](figures/[replace-with-actual-electricity-figure].png)

### Relationships between variables

[Summarize a grouped comparison or correlation finding. Explain that correlation does not establish causation.]

## 8. Key findings

Replace the placeholders below with **3–6 findings supported by the executed notebook**:

- **EPC:** [Most common rating and percentage or count].
- **Gas:** [Observed change between verified start and end years, with units].
- **Electricity:** [Observed change between verified start and end years, with units].
- **Building characteristics:** [One measured group difference or association].
- **Data quality:** [One quantitative result of cleaning or validation].

## 9. Limitations and biases

- The dataset has few missing data for building types, households or geographical areas; confirm the actual coverage.
- EPC ratings and measured consumption describe related but different aspects of building energy performance.
- Changes in energy consumption may also reflect weather, energy prices and occupancy; observed trends alone do not establish causes.

## 11. AI usage disclosure

**Tool:** ChatGPT (conversational assistance; not an autonomous agent editing the repository in this workflow).

**Why:** To understand Python and Git/GitHub workflows, troubleshoot installation and version-control issues.

**Where:** Assistance was used for learning Pandas, plotting approaches, Git branching and Pull Requests. 

**Lessons learned:** AI assistance can accelerate debugging and documentation, but its suggestions must be checked against the actual repository structure, dataset columns and intended notebook outputs.
