# ✈️ Animated Airline Route Visualization — Tableau

An animated geospatial dashboard built in **Tableau Desktop** comparing how **Delta** (hub-and-spoke) and **Southwest** (point-to-point) structure their U.S. route networks, and animating a full day of flight activity minute-by-minute.

## Skills Demonstrated
- **Geospatial visualization** — custom lat/long mapping with generated coordinate fields
- **Calculated fields** — Origin Point, Destination Point, and route sequencing logic
- **Custom mark shapes** — imported and oriented a custom airplane icon (straight / inverted) mapped to flight bearing
- **Animation & Pages shelf** — built a time-based "Pages" animation (`MINUTE(Clock)`) with playback controls and trail history
- **Data modeling** — worked with two linked data sources (`cleaned_flight_data.csv`, `interpolated_flight_paths.csv`) to interpolate flight paths between real ADS-B position pings
- **Comparative network analysis** — visually contrasted hub-and-spoke vs. point-to-point airline route models
- **Dashboard storytelling** — multiple worksheets combined into a cohesive narrative ("From Dawn to Dusk," "A Day in the Skies")

## Project Overview
Using real flight-tracking data, this project explores how airline route network design shows up visually:

- **Southwest Airlines** → point-to-point model — routes form a dense, decentralized web across the map
- **Delta Air Lines** → hub-and-spoke model — routes converge sharply on a central hub (Atlanta)

The final deliverable animates full-day flight movement for each airline, with trailing flight paths that build up over time to reveal network structure.

## Screenshots

### Setting up the custom airplane shape
![Airplane shape setup](images/Q1.png)

### Importing and configuring the flight path data source
![Data import](images/Q2.png)

### Calculated fields (Origin Point, Destination Point, Route)
![Calculated fields](images/Q3.png)

### Building the base route plot
![Route plot](images/Q4.png)

### Orienting airplane shapes to route bearing
![Airplane shape orientation](images/Q6.png)

### Hub-and-spoke vs. point-to-point comparison in motion
![Network comparison](images/Q7.png)

### Southwest Airlines — point-to-point network animation
![Southwest network](images/Q10.png)
![Southwest network dense](images/Q11.png)
![Southwest network full day](images/Q12.png)

### Delta Air Lines — hub-and-spoke network animation
![Delta network](images/Q13.png)
![Delta network tooltip detail](images/Q14.png)

## Tools & Data
- **Tool:** Tableau Desktop
- **Data:** ADS-B flight tracking data — `cleaned_flight_data.csv` (raw pings) and `interpolated_flight_paths.csv` (interpolated coordinates for smooth animation)
- **Workbook:** [`Data_Viz_Assignment_Animated_Visualization.twbx`](Data_Viz_Assignment_Animated_Visualization.twbx)

## Key Takeaway
Animation isn't just decoration here — the minute-by-minute build-up of flight paths makes the *structural difference* between the two network models immediately intuitive: Southwest's map fills in as a scattered web, while Delta's converges into a visible star pattern centered on its hub.
