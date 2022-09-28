# The Traveling Fulbrighter
## A program that calculates the shortest cycle of traveling from given destinations

Given a Fulbright student a starting point, they would enter destinations that they want to visit within the day.
The program would return a calculated cycle of ordered locations they should visit to minimize their traveling time.

### Required Libraries & APIs:
**Googlemaps:** 
is a web mapping service application provided by Google, offering geocoded locations, shortest path calculations, reverse geocoded locations..
For this particular project, I used:
* Geocoding: to convert addresses to geographic coordinates and vice versa.
* Distance matrix: to calculate the distances between different locations given coordinates.

**Folium:** 
helps visualizing data using a `leaflet.js' map.
* `folium.Map`creates a Googlemaps-like version given a centering location and zoom ratio.
* `folium.Marker` puts on the already drawn folium map markers given the destinations.

### The Process:
* Step 1: Retrieve access to Googlemaps API and prompts a list of destinations.
* Step 2: Calculate the distances for each pair of location and store them in a matrix.
* Step 3: Geocoding to get the coordinates of these location.
* Step 4: Mapping the intial map of locations.
* Step 5: Drawing on the traveling salesman problem, calculates all the possible tours through the destinations and return the shortest one.
* Step 6: Create a final map indicating the result.
