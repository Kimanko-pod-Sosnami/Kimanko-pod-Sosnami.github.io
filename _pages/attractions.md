---
layout: default
title: Kimanko pod Sosnami - Attractions
permalink: /attractions/
---

# Attractions

The center of [Brenna](https://en.wikipedia.org/wiki/Brenna,_Poland) is within walking distance of our Bed & Breakfast,
here you'll find various restaurants and shops. For people looking for a more active holiday, there are hiking trails 
starting from Brenna, while those travelling with children will be happy to find playground and activities for 
kids nearby. 

Here is a list of our suggestions:

## Places to eat

## Things to see

## Activities for children

## Sports: Hiking, cycling ...

<div id="map"></div>

<script>
  var map;
  function initMap() {
    map = new google.maps.Map(document.getElementById('map'), {
      center: {lat: 49.7186637, lng: 18.9394271},
      zoom: 13
    });

    /*function addMarker(props) {
      var marker = new google.maps.Marker({
        position: props.coords,
        map: map,
      });

      var infoWindow = new google.maps.InfoWindow({
        content: '<h2>' + props.name + '</h2><p>' + props.address + '</p><p><strong>Openingsuren:</strong></p><p>' + props.opening_hours + '</p>'
      });

      marker.addListener('click', function() {
        infoWindow.open(map, marker);
      });

    }

    $.getJSON( "pharmacy_data.json", function( data ) {
      data.forEach(function(el){
        addMarker(el);
      })
    });*/

  }
</script>
<script src="https://maps.googleapis.com/maps/api/js?key={{ site.maps_api_key }}&callback=initMap"
async defer></script>

