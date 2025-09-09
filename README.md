# Project README

## Overview
This project contains code, scripts, and resources for fitness test data analysis and related functionality.

## Included Components
- **Data Processing Scripts**: Tools to clean, validate, and prepare fitness testing data (PACER, Push-ups, Modified Pull-ups, etc.).
- **Business Rules**: Validation against CDC growth charts and FitnessGram standards.
- **Analysis Modules**: Code for statistical analysis and visualization of test results.
- **Documentation**: This README and supplementary references for FitnessGram and CDC resources.

## Business Rules
- When entering data into the database, verify values fall within the valid range for the individual's age and gender by referencing the **CDC Growth Chart**.
- For PACER test scores, valid range: **1–247 laps**.
- For Push-Ups and Modified Pull-Ups, valid range: **0–75 repetitions** (system cap).

## Usage
1. Clone this repository or download the source files.
2. Install dependencies listed in `requirements.txt` (if applicable).
3. Run data processing scripts on your dataset using Python 3.8+.
4. Review outputs in the `results/` folder.

## References
- [FitnessGram Test Administration Manual](https://dl.icdst.org/pdfs/files/2801e301e713d36f204bd16b56d7055b.pdf)
- [CDC Growth Charts](https://www.cdc.gov/growthcharts/)
- [PACER Test Details - Wikipedia](https://en.wikipedia.org/wiki/Multi-stage_fitness_test)

---
*Prepared for internal project documentation purposes.*
