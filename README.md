# Dementia Detection Using Eye Tracking

## Project Overview

This project utilizes eye-tracking data to detect potential signs of dementia. By analyzing eye movement patterns, including blinks, fixations, and saccades, the project aims to provide insights into cognitive health. The analysis focuses on metrics such as saccade duration, pupil diameter, and fixation counts.

## Project Structure

- `data/` - Contains raw eye-tracking data files.
- `scripts/` - Includes Python scripts for data processing and analysis.
  - `preprocessing.py` - Functions for removing missing data.
  - `blink_detection.py` - Functions for detecting blinks.
  - `fixation_detection.py` - Functions for detecting fixations.
  - `saccade_detection.py` - Functions for detecting saccades.
  - `analysis.py` - Script to perform the main analysis and generate results.
- `results/` - Output data and analysis results.
- `visualizations/` - Graphs and charts for visualizing the results.


## Functions
- `remove_missing(x, y, time, missing):` Removes missing data points from the input arrays.
- `blink_detection(x, y, time, missing=0.0, minlen=10):` Detects blink events in the eye-tracking data.
- `fixation_detection(x, y, time, missing=0.0, maxdist=25, mindur=50):` Identifies fixation events based on distance and duration.
- `saccade_detection(x, y, time, missing=0.0, minlen=5, maxvel=40, maxacc=340):` Detects saccades using velocity and acceleration thresholds.


## Requirements

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
