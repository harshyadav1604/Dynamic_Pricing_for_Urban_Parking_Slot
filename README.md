# Dynamic_Pricing_for_Urban_Parking_Slot

Project Overview:
This project analyzes urban parking lot occupancy data to understand usage patterns and predict Dynamic Pricing of each lot.  The dataset contains information about parking lot including capacity, real-time occupancy, vehicle types, traffic conditions, and timestamps. 
The aim is to provide insights into parking space utilization and help optimize parking management.

Teck Stack:
Python: Primary programming language.
Pandas: Data manipulation and analysis.
NumPy: Numerical computations.
Matplotlib/Seaborn: Data visualization.
Pathway: Real-time data processing.
Bokeh/Panel: Interactive visualizations.

graph TD
    A[Raw Parking Data] --> B[Data Loading]
    B --> C[Data Preprocessing]
    C --> D[Feature Engineering]
    D --> E[Time Series Analysis]
    D --> F[Occupancy Rate Calculation]
    E --> G[Visualization]
    F --> G
    G --> H[Insights & Predictions]

Project Architecture and Workflow:

1) Data Loading: 
The dataset is loaded from a CSV file containing urban parking lot data.
Key fields include ID, SystemCodeNumber, Capacity, Occupancy, Vehicle Type, TrafficConditionsNearBy, Timestamps etc.

2) Data Preprocessing:
Handling missing values (though none were found in      this dataset).
Creating a parking lot Id based upon SystemCodeNumber.
Sorting data by timestamp for time series analysis.
Mapping vehicle types to weights for weighted occupancy calculations.

3) Feature Engineering:
Datetime stamp is formed by merging Date and Time stamp.
Added vehicle weight mapping (bike=0.5,  car=1, truck=1.5).
Calculated occupancy rate (Occupancy/Capacity).

4) Analysis Capabilities:
Time-based occupancy patterns (hourly, daily, weekly trends).
Parking lot comparison by prices.

5) Visualization:
    Time series plots of prices.
    Interactive dashboards for exploration.


