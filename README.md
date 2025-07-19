#  Delhi Traffic ML App: Least Congested Route Finder

This app uses **Machine Learning and OpenStreetMap data** to find the **least congested (fastest)** route between any two locations in Delhi.  

It leverages real traffic speed datasets and dynamically builds the road network for route optimization.

---

##  Screenshot

![App Screenshot](Screenshot%202025-07-19%20232841.png)

---

##  Features

 Find least congested routes between any two Delhi locations  
 Uses real traffic speed data from `2024_week_day_speed_city.csv`  
 Dynamically downloads the Delhi road network from OpenStreetMap  
 Visualizes the route on an interactive map (HTML)  
 Automatically opens the route map in your browser  

---

##  How It Works

1. Enter **Start Location** (e.g., `"India Gate, Delhi"`)  
2. Enter **End Location** (e.g., `"Jama Masjid, Delhi"`)  
3. The app:
   - Loads the Delhi road network
   - Applies traffic speed data for the selected day
   - Computes the fastest path
4. Generates an interactive map showing your route.  

The map is saved at:
C:\Users\sagni\Downloads\Road Traffic\delhi_dynamic_least_congested_route.html

yaml
Copy
Edit

---

##  Dependencies

- Python 3.11+
- pandas
- geopandas
- osmnx
- networkx
- folium

Install them with:
```bash
pip install pandas geopandas osmnx networkx folium
 Dataset Used
 2024_week_day_speed_city.csv
Contains average speeds (in km/h) for each day of the week in Delhi.

