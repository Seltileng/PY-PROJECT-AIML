# Plateau State Geographical Electoral Analysis

A Python-based geographical and statistical analysis of polling unit election results across **Plateau State, Nigeria**.

The project uses polling unit results, geographical coordinates, and spatial analysis techniques to investigate voter participation, turnout, party support, electoral competition, outliers, and geographical relationships between polling units.

---

## 📌 Project Objectives

The main objective is to understand how electoral results vary geographically across Plateau State.

The analysis focuses on:

- Voter participation across Local Government Areas (LGAs)
- Polling unit voter turnout
- Geographical distribution of political party support
- Total votes across LGAs
- Patterns of party dominance
- Electoral outliers
- Electoral competitiveness
- Similarity between geographically close polling units
- Completeness and reliability of polling unit results
- Areas requiring improved electoral data collection and monitoring

---

## 🔎 Research Questions

The project addresses the following questions:

1. Which LGAs recorded the highest and lowest voter participation rates?
2. Which polling units had the highest voter turnout, and where are they geographically located?
3. Where did each major political party have the strongest support across Plateau State?
4. Which LGAs recorded the highest number of total votes, and what factors may explain their performance?
5. Are there geographical patterns in party dominance across Plateau State?
6. Which polling units are electoral outliers based on unusually high/low turnout or extreme party vote concentration?
7. Which areas recorded the highest level of electoral competition based on the difference between the winning party and the second-highest party?
8. Do polling units located close to each other show similar voting patterns?
9. Which LGAs have the most complete and reliable polling unit result records?
10. Which geographical areas may require more attention for future electoral data collection and monitoring?

---

# 🛠️ Methodology

The project follows a multi-stage analytical workflow.

## 1. Data Collection

Polling unit election results are collected and organized into a structured dataset.

The dataset may contain:

- Polling unit name/code
- Ward
- LGA
- Registered voters
- Accredited voters
- Total votes
- Valid votes
- Invalid/rejected votes
- Votes received by political parties
- Polling unit location

---

## 2. Data Cleaning

Python is used to:

- Remove duplicate records
- Handle missing values
- Standardize LGA and polling unit names
- Validate numerical fields
- Identify incomplete records
- Check for inconsistent vote totals
- Prepare the dataset for geographical analysis

---

## 3. Coordinate Generation

Before the main analysis, each polling unit will be assigned geographical coordinates:

- Latitude
- Longitude

The coordinates will be used to represent polling units geographically across Plateau State.

Coordinates will also be checked for:

- Missing locations
- Duplicate coordinates
- Invalid coordinates
- Incorrect locations
- Unusually distant locations

---

## 4. Geographical Analysis

The polling units will be converted into geographical data using **GeoPandas**.

This allows the project to analyze:

- Polling unit locations
- LGA boundaries
- Party support by location
- Turnout distribution
- Spatial clusters
- Geographical outliers
- Relationships between nearby polling units

---

# 📊 Electoral Analysis

## Voter Participation

Voter participation will be calculated using:

```text
Participation Rate =
Accredited Voters / Registered Voters × 100
