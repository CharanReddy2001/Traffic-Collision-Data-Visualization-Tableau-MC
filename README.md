# Traffic Collision Data Analysis: Enhancing Road Safety in Montgomery County

## Overview
This project analyzes traffic collision data from Montgomery County, Maryland, to identify patterns, accident hotspots, and factors influencing road safety. The goal is to use data visualizations and insights to inform decision-making for improving road safety and reducing traffic-related incidents.

## Dataset Description
The dataset contains detailed information on 172,105 traffic accidents that occurred on county and local roads within Montgomery County. The data spans 43 columns and was sourced from the Maryland State Police's Automated Crash Reporting System.

**Key Features:**
- `Report Number`: Unique identifier for each collision report.
- `Crash Date/Time`: Date and time when the collision occurred.
- `Route Type`: Type of road (e.g., Maryland State, County).
- `Collision Type`: Type of collision (e.g., rear-end, head-on).
- `Weather`: Weather conditions at the time of the collision.
- `Traffic Control`: Type of traffic control (e.g., traffic signal).
- `Injury Severity`: Severity of injuries sustained in the collision.
- `Driver Distracted By`: Factors distracting the driver at the time of the collision.
- `Vehicle Make`: Manufacturer of the vehicle involved.

## Data Source
The data was collected from the Crash Reporting - Drivers Data dataset on Data.gov, sourced from the Maryland State Police's Automated Crash Reporting System.

**Source**: [Crash Reporting - Drivers Data](https://catalog.data.gov/dataset/crash-reporting-drivers-data)

## Preprocessing Steps
1. **Identifying Missing Values**: Used `isnull()` and `.sum()` to check for missing values across the dataset.
2. **Handling Missing Values**: 
   - Replaced missing values in key columns (e.g., `Collision Type`, `Weather`, `Traffic Control`) with the most common values.
   - Converted date/time columns to proper datetime formats.
   - Standardized inconsistent vehicle make values.
3. **Feature Engineering**: Cleaned data and resampled for ease of analysis using machine learning algorithms.
4. **Reverification**: Ensured there were no missing values in the cleaned dataset.

## Exploratory Data Analysis (EDA)

### Visualizations:
1. **Accidents by Route Type**: A waffle chart showing the distribution of accidents by route type.
   - **Insight**: Maryland state roads are the most common location for accidents (44.93% of the total incidents).
   
2. **Vehicle Make Frequency**: A word cloud illustrating the frequency of different vehicle makes involved in accidents.
   - **Insight**: Toyota, Honda, Chevy, and Ford are the most commonly involved car manufacturers.

3. **Accident Hotspots in Montgomery County**: A choropleth map showing the geographical distribution of accidents.
   - **Insight**: State highways in Maryland are accident hotspots.

4. **Accidents by Vehicle Manufacturing Year**: A bar graph displaying the frequency of accidents based on vehicle manufacturing year.
   - **Insight**: The highest number of accidents occurred with vehicles manufactured between 2013 and 2019.

## Key Insights
- **Accident Trends by Year**: Significant trends in accident frequency over the years with a marked increase in 2017.
- **Driver Behavior**: Many accidents are caused by driver errors, with no obvious injuries being the most common outcome.
- **Third-Party Involvement**: Pedestrian interference is a key factor in accidents involving third parties.
- **Weather and Vehicle Age**: Weather conditions and vehicle age influence the frequency and severity of accidents.
- **Speed Limit and Severity**: The speed limit on roads, particularly those with 35 mph limits, affects both the frequency and severity of accidents.

## Smart Questions Addressed
- **How many accidents occur annually in Montgomery County?**: Annual accident counts and their severity are presented through a bar chart.
- **What role do drivers play in accidents?**: Most accidents are driver-related, often caused by distracted or impaired driving.
- **What factors contribute to accidents?**: Weather, vehicle age, and driver substance use were found to influence accidents.
- **Do speed limits affect accident severity?**: Accidents on roads with 35 mph speed limits are prevalent, suggesting a need for better speed enforcement.

## Challenges
- Limited utilization of all available data rows due to the dataset's size.
- Presence of numerous missing values required extensive preprocessing.

## Future Directions
- **Machine Learning Integration**: Implement machine learning techniques for predictive analysis, anomaly detection, and deeper insights.
- **More Data**: Incorporate additional data sources for enhanced analysis (e.g., road infrastructure data).

## Lessons Learned
- Extensive data preprocessing and cleaning are essential for meaningful analysis.
- Visualizations should be simplified for better clarity and insights.
- Data-driven decisions can significantly inform policies to improve road safety.

## Conclusion
This analysis provides key insights into traffic accidents in Montgomery County, with particular focus on pedestrian involvement, road conditions, and speed limits. Targeted interventions, such as improved pedestrian safety measures and enforcing speed limits, can help reduce the occurrence and severity of traffic collisions.

## Repository Structure
📂 Data/ # Processed dataset files

📂 Notebooks/ # Jupyter notebooks for preprocessing and analysis

📂 Visualizations/ # Tableau visualizations and plots

📄 README.md # Project documentation (this file)

📄 report.pdf # Final project report

## 📜 License  
This project is licensed under the **MIT License**.  

**MIT License**  

This project is licensed under the **MIT License** – you are free to use, modify, and distribute it under the terms of the license.  
