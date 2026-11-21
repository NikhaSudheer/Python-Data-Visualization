PROJECT DOCUMENTATION -- Python Data Visualization

PROJECT OVERVIEW

This project analyzes New York City taxi trips using Python to clean the data and visualize fares, tips, distances and payment methods across pickup boroughs, helping understand how trip patterns and costs vary.

TOOLS USED

1.Python

2.Pandas

3.Matpotlib

4.Seaborn

DATASET

sns.load_dataset("taxis")

Data contains : Pickup and dropoff time, Passengers, Distance, Fare, Tip, Tolls, Total, Payment method, Pickup and dropoff zone, Pickup and dropoff borough, etc.

STEPS FOLLOWED

*Loaded the taxis dataset using Seaborn

*Checked for missing values (found only in payment, pickup_zone, dropoff_zone, pickup_borough and dropoff_borough)

*Imputed missing values by column type (median for numerical columns, mode for categorical columns)

*Removed rows with missing pickup_zone or pickup_borough, since these critical columns cannot be reasonably imputed (6,433 → 6,407 rows)

*Built visualizations using Matplotlib: line chart, bar chart, pie chart, histogram and box plot

*Built visualizations using Seaborn: count plot, scatter plot, heatmap, pair plot and violin plot

KEY INSIGHTS

*Manhattan dominates the data, with 5,268 of 6,407 trips and the highest total fare (about 58,750).

*Credit card is the main payment method (71.8% of trips, against 28.2% cash), and cash trips show no tips, so cash tips appear not to be recorded.

*Most trips are short (median distance about 1.65 miles), so the distance histogram is strongly right-skewed.

*Fare is strongly correlated with distance (0.94) and with total (0.97), while tip has a much weaker correlation with fare and distance (about 0.47).

FILES INCLUDED

1)Python Data Visualization.ipynb - Jupyter Notebook with codes

2)README.md - Project Description

