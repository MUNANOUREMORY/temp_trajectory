#Temperature trajectory subphenotypes
Objective
Retrospective multi-hospital study using the CLIF framework to analyse the hospital wide differences in subphenotypes' independent relationships with hospital mortality and bloodstream infection using multivariable models. The models are published in an existing study - Temperature Trajectory Subphenotypes in Oncology Patients with Neutropenia and Suspected Infection

You will need most recent icu_cohort.csv from mortality_model code.

RCLIF 2.0 Tables required:
clif_hospitalization
clif_patient
clif_adt (location_category == "icu")
clif_respiratory_support (device_category == "imv")
clif_vitals (vital_category == "temp_c)

Follow the schema laid out in the RCLIF ERD for each of these tables.

Setup instructions
Step 1. Before running temperature_trajectory_analysis, make sure you have ran mortality_model code.
Step 2. Make sure to input site specific details at the top of the R file BEFORE running. No need to load config or any other file.
Step 3. Run the temperature_trajectory_analysis.R analysis script. This script generates and saves aggregate results in the current directory.
Step 4. Please upload all outputs to Box (https://app.box.com/folder/296487589366)
