## Folium

#### Folium builds on the data wrangling strengths of the Python ecosystem and the mapping strengths of the Leaflet.js library. Manipulate your data in Python, then visualize it in a Leaflet map via folium.

* Installation of the **package:**

`pip install folium`

* To create a base map, simply pass your starting coordinates to Folium:

Usage:

```python
import folium
m = folium.Map(location=[45.5236, -122.6750])
```
```python
m.save("index.html")
```
```python
m = folium.Map(location=[45.372, -121.6972], zoom_start=12, tiles="Stamen Terrain")

tooltip = "Click me!"
folium.Marker(
    [45.3288, -121.6625], popup="<i>Mt. Hood Meadows</i>", tooltip=tooltip
).add_to(m)
```
