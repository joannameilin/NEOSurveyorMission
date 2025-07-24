## NEOSurveyor_fulldigest2.ipynb

Runs digest2 on provided .xml files and creates a breakdown of all score categories, formatted as a .csv file. Matches trksubs with designations to remove noisy tracklets/observations that do not belong to a real object. Directories (located in second cell block) should be modified to the user's desktop/file configuration.

## NEOSurveyor_Data_analysis.ipynb

Matches trksubs to designations (removed noisy tracklets). Generates **three types of .csv files:** 
> .digest2: shows digest2 score breakdowns, same as NEOSurveyor_fulldigest2.ipynb)

> .digest2_filter: trksubs formatted for optimal threshold filtering. Last column is titled "class." Class = 0 indicates NEO, class =  indicates MBA

> .digest2_ml: trksubs formatted for machine learning models. Last column is titled "orbtype." Orbtype = 0 indicates NEO, orbtype = 1 indicates MBA

This notebook also runs the optimal thresholds and machine learning code if needed and analyzes the results. Will print the number of NEOs mistaken as MBAs in the optimal thresholds and print ML results while saving ML confusion matrices to the user's desktop. 

## NEOSM_Data_Visualization
Creates interactive density heatmaps given large digest2 score breakdown files (in csv format). 
