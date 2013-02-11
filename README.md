<!DOCTYPE html>
<html>
<head>
<script
src="http://maps.googleapis.com/maps/api/js?key=AIzaSyBc8bajxwz0YkqF12U_FHhAU8qqOFIAgFY&sensor=false">
</script>

<style type="text/css">
html, body {width: 100%; height: 100%}
    body {margin-top: 0px; margin-right: 0px; margin-left: 0px; margin-bottom: 0px}
</style>

<script>
var myCenter=new google.maps.LatLng(38.437163,-78.868018);

function initialize()
{
var mapOptions = {
  center:myCenter,
  zoom:5,
  mapTypeId:google.maps.MapTypeId.HYBRID
};
var map=new google.maps.Map(document.getElementById('googleMap'),mapOptions);

var marker = new google.maps.Marker({
  position:myCenter,
});

marker.setMap(map);
}

google.maps.event.addDomListener(window, 'load', initialize);
</script>
</head>

<body>
<div id="googleMap" style="width:100%;height:100%;"></div>
</body>
</html>
