# Surfs_Up - Module 9 Challenge

## Overview of the Analysis

The overview of this analysis was to review weather data and prepare a business plan in order to entice an investor, W. Avy to provide financial backing for a surf and shake shack that we are interested in opening in Hawaii.  By using SQLite, specifically SQLAlchemy in connection with Pandas and Jupyter Notebook, we were able to query the data from a specific source file and provide cohesive results in the form of Pandas DataFrames.


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
