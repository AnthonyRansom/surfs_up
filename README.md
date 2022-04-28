# surfs_up

## Overview of Project

### Purpose

This will provide insights into the temperature trends of the Oahu area in Hawaii in order to
provide insight into he sustainability to operate an ice cream shop business year-round.

## Results

### Comparison of June and December Temperatures

From the review of the data the following has been determined:
 - The data shows less temperature reading for the month of December with only 1517 readings considering December has more days than June with June showing 1700 Temperature readings
 - The average temperature for June and December is within a 4 degree difference
 - There is a significant difference between the minimum temperatures with June showing a minimum of 64 and December a minimum of 56

<img src="Resources/june_temps.PNG" width="166" height="245"> <img src="Resources/December_temps.PNG" width="166" height="245">

## Summary

### High Level Summary

From the analysis above the summary of the temperature data indicates there is no significant difference in
temperature when comparing the half year June and end year December results.

### Additional Analysis
The following two additional queries would gather the data for precipitation for the month of June and December in order
to provide insight into the weather conditions for the months of June and December in the Oahu region
#### June Precipitation
 - june_prcp = session.query(Measurement.prcp).filter(func.strftime("%m", Measurement.date) == '06').all()
 
#### December Precipitation
 - dec_prcp = session.query(Measurement.prcp).filter(func.strftime("%m", Measurement.date) == '12').all()

