The Algae Platform London will map the actors and resources in the bio region of London. 

### Support or Contact

please send an email to samuel.iliffe@network.rca.ac.uk for any comments on the project.


<!DOCTYPE html>
<html>
<head>
<meta charset='utf-8' />
<title>Attach a popup to a marker instance</title>
<meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
<script src='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.js'></script>
<link href='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.css' rel='stylesheet' />
<style>
body { margin: 0; padding: 0; }
#map { position: absolute; top: 0; bottom: 0; width: 100%; };
</style>
</head>
<body>
<style>
 
#marker {
background-image: url('https://docs.mapbox.com/mapbox-gl-js/assets/washington-monument.jpg');
background-size: cover;
width: 50px;
height: 50px;
border-radius: 50%;
cursor: pointer;
}
 
.mapboxgl-popup {
max-width: 200px;
}
 
</style>
 
<div id='map'></div>
 
<script>
mapboxgl.accessToken = 'pk.eyJ1IjoiZHVzdGRlbGVnYXRpb24iLCJhIjoiY2pta2Z0NTc4MDBnYTNybzB2MGJ3ajFmcyJ9.z1fpWch_VYv-y4hmREoB-A';
 
var monument = [-77.0353, 38.8895];
var map = new mapboxgl.Map({
container: 'map',
style: 'mapbox://styles/mapbox/light-v10',
center: monument,
zoom: 15
});
 
// create the popup
var popup = new mapboxgl.Popup({ offset: 25 })
.setText('Construction on the Washington Monument began in 1848.');
 
// create DOM element for the marker
var el = document.createElement('div');
el.id = 'marker';
 
// create the marker
new mapboxgl.Marker(el)
.setLngLat(monument)
.setPopup(popup) // sets a popup on this marker
.addTo(map);
 
</script>
 
</body>
</html>
