# Task 2: Data Version Control (DVC) Setup

## Overview
In this task, I set up Data Version Control (DVC) to track the key data files used in the car insurance analytics project. This enables reproducibility, efficient storage, and versioning of large data files outside of Git.

## Files Tracked with DVC
- `data/cleaned_data.csv`: The main cleaned dataset containing historical insurance claim data.
- `data/MachineLearningRating_v3.txt`: Additional data file used for machine learning model ratings and evaluations.

## Steps Taken
1. Initialized DVC in the project repository.
2. Added the data files to DVC tracking using:
   ```bash
   dvc add data/cleaned_data.csv
   dvc add data/MachineLearningRating_v3.txt
