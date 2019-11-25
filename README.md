The Algae Platform London will map the actors and resources in the bio region of London. 

### Support or Contact

please send an email to samuel.iliffe@network.rca.ac.uk for any comments on the project.


<!DOCTYPE html>
<html>
<head>
<meta charset='utf-8' />
<title>Display a map with a custom style</title>
<meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
<script src='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.js'></script>
<link href='https://api.tiles.mapbox.com/mapbox-gl-js/v1.5.0/mapbox-gl.css' rel='stylesheet' />
<style>
body { margin: 0; padding: 0; }
#map { position: absolute; top: 0; bottom: 0; width: 100%; };
</style>
</head>
<body>
<div id='map'></div>
<script>
mapboxgl.accessToken = 'pk.eyJ1IjoiZHVzdGRlbGVnYXRpb24iLCJhIjoiY2pta2Z0NTc4MDBnYTNybzB2MGJ3ajFmcyJ9.z1fpWch_VYv-y4hmREoB-A';
var map = new mapboxgl.Map({
container: 'map', // container id
style: 'mapbox://styles/mapbox/dark-v10', //hosted style id
center: [-77.38, 39], // starting position
zoom: 3 // starting zoom
});
</script>
 
</body>
</html>
