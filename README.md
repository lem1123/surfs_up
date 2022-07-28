# Surfs_Up - Module 9 Challenge

## Overview of the Analysis

The overview of this analysis was to review weather data 


## Results

*** 

* Weather Results for June

```

june_results = session.query(Measurement.date, Measurement.tobs).filter(extract("month", Measurement.date) == 6)

```

```
june_results = session.query(Measurement.date, Measurement.tobs).filter(extract("month", Measurement.date) == 6).all()

```

![June_Temps.png](June_Temps.png)


* Weather Results for December 

```

dec_results = session.query(Measurement.date, Measurement.tobs).filter(extract("month", Measurement.date) == 12).all()

```

![December_Temps.png](December_Temps.png)


## Summary

In conclusion, it appears that the weather data provided for the temperatures in June and December are not that different.  
