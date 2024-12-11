### **Temperature trajectory subphenotypes**
# **Objective**
Retrospective multi-hospital study using the CLIF framework to analyse the hospital wide differences in subphenotypes' independent relationships with hospital mortality and bloodstream infection using multivariable models. The models are published in an existing study - Temperature Trajectory Subphenotypes in Oncology Patients with Neutropenia and Suspected Infection

You will need most recent icu_cohort.csv from mortality_model code.

# **RCLIF 2.0 Tables required:**
- clif_hospitalization
* clif_patient
+ clif_adt (location_category == "icu")
- clif_respiratory_support (device_category == "imv")
* clif_vitals (vital_category == "temp_c)

Follow the schema laid out in the RCLIF ERD for each of these tables.

# **Setup instructions**
* Step 1. Rename `config_template.json` to `config.json` and update the required details.
* Step 2. Before running, please contact sivasubramanium.bhavani@emory.edu for numeric coefficients (lines 146-150)
* Step 2. Run `ICU_cohort_id_script_CLIF 2.0.R`. This script generates table1 and an intermediate dataset.
* Step 3. Run `the temperature_trajectory_analysis_2.0.R` analysis script. This script generates and saves aggregate results in the current directory.
* Step 4. Please upload all outputs to [Box](https://app.box.com/folder/296487589366)
