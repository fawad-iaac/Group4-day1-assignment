# Group 4 — Data Cleaning and Exploratory Data Analysis

## Team Members
- Daria
- Fawad
- Hetashri
- Luis

## Project Overview

This project focuses on cleaning, preprocessing, and performing Exploratory Data Analysis (EDA) on property-level energy consumption data.

The analysis explores electricity and gas consumption patterns, Energy Performance Certificate (EPC) distributions, and differences in energy consumption across property types.

## Dataset

**Dataset:** National Energy Efficiency Data-Framework (NEED): anonymised data 2026

**Publisher:** UK Department for Energy Security and Net Zero

**Publication date:** 11 June 2026

**Dataset description:** Property-level data containing gas and electricity consumption from 2005 to 2024, property characteristics, and energy-efficiency measure installations.

**Official publisher:** [Department for Energy Security and Net Zero](https://www.gov.uk/government/organisations/department-for-energy-security-and-net-zero)

### Local Dataset

The notebook reads the anonymised dataset from:

data/anon2026_50k.csv

## Project Structure

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
