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

* To `save` the output map

Usage:

```python
m.save("index.html")
```

* The default tiles are set to `OpenStreetMap`, but `Stamen Terrain`, `Stamen Toner`, `Mapbox Bright`, and `Mapbox Control Room`, and many others tiles are built in.

Usage:

```python
m = folium.Map(location=[45.372, -121.6972], zoom_start=12, tiles="Stamen Terrain")

tooltip = "Click me!"
folium.Marker(
    [45.3288, -121.6625], popup="<i>Mt. Hood Meadows</i>", tooltip=tooltip
).add_to(m)
```
