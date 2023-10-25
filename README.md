# MIMIC-IV-Hip-Fracture-Mortality-Prediction

This code corresponds to the paper "Machine learning‐based mortality prediction in hip fracturepatients using biomarkers" (https://onlinelibrary.wiley.com/doi/epdf/10.1002/jor.25675?domain=author&token=HNGVUWNIEST7YKKQN9ZR)

The python code in this repository was used to prepare lab data for input into machine learning models, sourced from the MIMIC-IV database (primarily from the labevents.csv and patients.csv files in the hosp module). 

The data table was cleaned outside code in Excel by imputing means where blanks existed, ignoring lab test columns that were nearly entirely populated by blanks, and selecting 1 record for each patient (whereas the starting dataset included multiple admissions for each patient). 

The Pycaret library was used to assess how various machine learning algorithms perform at the task of predicting mortality within 1, 5, and 10 years of a hip fracture based on lab test values and demographic characteristics at the time of the hospital admission. Pycaret can be installed with "pip install pycaret". 
