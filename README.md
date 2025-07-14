# TUB-ReproCogsci
This repository contains analysis scripts used in module "Digital Tools for Reproducible Research in Cognitive Science" offered at TU Berlin.
It contains scripts restructuring and processing a publicly shared data set for training purpose.

# About this Repository
This repository was created as part of the "Digital Tools for Reproducible Research" course at TU Berlin.
The original scripts were developed by Sein Jeung and adapted by Mathewos Ayele Gugsa for use with a specific dataset.

# What the Scripts do
1. gaits_01_import.py
- Loads raw force plate data (.txt) for multiple participants.
- Extracts relevant columns (time, left/right foot force).
- Saves cleaned .tsv files in folder structure.
- Also creates basic plots of vertical ground reaction forces.

2. gaits_02_extract_features.py
- Detects gait events like rising/falling edges and final contacts.
- Calculates stride times for left and right foot.
- Outputs stride time tables (_strides.tsv) and visualization figures.

3. gaits_03_summary.py
- Loads stride times per participant.
- Calculates and plots average stride times for control vs. patient groups.
- Visualizes left vs. right foot data

# Dataset 
Data set : https://physionet.org/content/gaitpdb/1.0.0/
This is the dataset i worked with. I worked with the participants starting with `Ga`

# How to Run
- Update paths: Change the file paths at the top of each script to match your system (currently set for Windows).
- Install dependencies:
You’ll need numpy, matplotlib, and os..
- Run scripts in order:
1. gaits_01_import.py
2. gaits_02_extract_features.py
3. gaits_03_summary.py
Each script can be run directly in a Python environment 
