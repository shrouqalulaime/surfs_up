# surfs_up

## Project Overview
The goal of the project to anlayze the temprature trends at holidays months (mainly June and Decemnber) at Hawaii to determine if the surf and ice cream shop business is sustainable year-round. Two main anlaysis are done:
- Determine the temprature summary statistics for June
- Determine the temprature summary statistics for December

## Results:
- The average temprature at June is higher than at December by about 4 degrees, 75 and 71 F, respectively
- The varitions of the temprature data in both June and December are small ranging between 3.2 to 3.7, this might be attributed for the large smaple size obtained in each month, which is greater than 1500 observations
- The minimum temprature is observed at December (about 56 F), which is 8 degree lower than June

## Summary:
- Based on the analysis, the average temprature at December is very comparable to June ranging between 71 to 75, which means the surf and ice cream shop business can be sustainable year-round. 
- To collect more weather data for June and December, two other queries can be added:
1. Collect precipitation data: session.query(Measurement.prcp).filter(extract('month', Measurement.date)==6).all()
2. Collect station data to check measuments for most active station: session.query(Measurement.station).filter(extract('month', Measurement.date)==6).all()