# Geolocation and Mapping with Python (Geopy & Folium)

This project demonstrates how to leverage the power of Python libraries geopy and folium to:

* Convert a textual address (like "Lonavala") into its corresponding latitude and longitude coordinates.
* Generate a map centered on the geocoded location using Folium.
* Add a marker to the map pinpointing your specified coordinates.
  
**Installation:**

Ensure you have Python installed.

Install the required libraries using pip:
pip install geopy folium

**Running the Script:**

Open a Python interpreter (e.g., Jupyter Notebook, command prompt).
Copy and paste the provided code snippet into your environment.
Replace "Lonavala" with the address you want to geocode.
Execute the code cells or script.

**Explanation:**

* Import Libraries:

geopy.geocoders.Nominatim: Provides functionalities for geocoding addresses.
folium: Enables interactive map creation.
Geocoding the Location:

* Creates a Nominatim geolocator object with a user agent string (optional for attribution).
Uses geocode to convert the address ("Lonavala") into a Location object containing latitude and longitude.
Prints the extracted coordinates for verification.
Creating the Map:

* Initializes a folium.Map object centered at the geocoded coordinates ([latitude, longitude]).
Sets an initial zoom level (zoom_start=13) to provide a detailed view.
Marking Your Location:

* Defines the coordinates as a list (point).
Creates a folium.Marker object at the specified point (point).
Adds a popup label ('My City') to appear when clicking the marker.
Customizes the marker's appearance with folium.Icon() (optional - explore Folium's documentation for different icons).
Adds the marker to the map (mylocation.add_to(map)).

* Saving the Map:
Saves the generated map as an HTML file ("mylocation.html"). You can open this file in a web browser to view the interactive map.
Error Handling (in your provided code):

* Additional Notes:

Experiment with different addresses and explore Folium's capabilities for customizing maps (e.g., adding tiles, markers, popups, etc.).
Refer to the official documentation for geopy (https://geopy.readthedocs.io/) and folium (https://github.com/python-visualization/folium) for more advanced usage.

* Output:


![Screenshot 2024-06-21 134735](https://github.com/Vaishnavi639/geopy-folium-visualization/assets/127540530/c8baff04-ea28-4a2f-a6e3-eea7afd2f4e3)
