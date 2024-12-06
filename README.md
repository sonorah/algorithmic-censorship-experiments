# High Profile Cases Dataset: Data Cleaning and Analysis

This repository contains a Python script for analyzing social media content moderation cases. The script processes the dataset, extracts insights, and generates detailed reports to identify trends and patterns.

## Features

1. **Data Cleaning**:
   - Standardizes durations (e.g., "Permanent" or "Temporary").
   - Parses and validates dates.
   - Handles missing and malformed data gracefully.

2. **Analysis**:
   - Categorizes cases based on suspension reasons (e.g., "hate speech," "misinformation").
   - Tracks account types (verified accounts, political figures, journalists).
   - Identifies accounts with repeated suspensions.
   - Generates statistics like case frequency by month.

3. **Reporting**:
   - Creates summary reports for easy interpretation of results.
   - Splits analysis into pre- and post-October 2022 cases for temporal comparison.

## Contents

- `twitter_high_profile_suspensions.ipynb`: The main Python script for data cleaning and analysis.
- `Twitter_Suspensions.csv` (included): Dataset used in the analysis; data originates from [here](https://en.wikipedia.org/wiki/Twitter_suspensions).

## Requirements

- Python 3.8+
- Pandas
- A dataset (`Twitter_Suspensions.csv`) containing:
  - `Date`: Suspension date in "DD Month YYYY" format.
  - `Duration`: Suspension duration.
  - `Reason for suspension`: Description of the suspension reason.
  - `Description`: Account description.
  - `Individual/account`: Account name or identifier.
