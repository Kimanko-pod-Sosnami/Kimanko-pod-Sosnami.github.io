---
layout: default
title: Kimanko pod Sosnami - Contact
permalink: /contact/
---

# Contact

<div class="columns">
<div class="container column is-6">
<div class="card">
  <div class="card-image">
    <figure class="image is-4by3">
      <img src="{{ site.baseurl }}{{ site.header_image }}" alt="The guesthouse">
    </figure>
  </div>
  <div class="card-content">
    <div class="media">
      <div class="media-content">
        <p class="title is-4">Kimanko pod Sosnami</p>
        <p class="subtitle is-6">Bed and Breakfast</p>
      </div>
    </div>

    <div class="content">
      <p>{{ site.data.contact.address.street_number }}<br />{{ site.data.contact.address.municipality }}<br />{{ site.data.contact.address.country }}</p>
      <p><span class="icon"><i class="fas fa-envelope"></i></span> <a href="mailto:{{ site.data.contact.email }}">{{ site.data.contact.email }}</a></p>
      <p><span class="icon"><i class="fas fa-phone"></i></span> {{ site.data.contact.tel }}</p>
    </div>
  </div>
</div>
</div>
<div class="container column is-6">
    <div id="map" class="card is_fullheight"></div>
</div>

</div>


## How to get to our guesthouse ?

### By Car

### By Bus

### By Train

### By Plane




<script>
  var map;
  function initMap() {
    map = new google.maps.Map(document.getElementById('map'), {
      center: {lat: 49.7186637, lng: 18.9394271},
      zoom: 15
    });

    function addMarker(props) {
      var marker = new google.maps.Marker({
        position: props.coords,
        map: map,
      });

      var infoWindow = new google.maps.InfoWindow({
        content: '<p>It is here</p>'
      });

      marker.addListener('click', function() {
        infoWindow.open(map, marker);
      });

    }

    addMarker({
        coords: {lat: 49.7186637, lng: 18.9394271},
    });

  }
</script>
<script src="https://maps.googleapis.com/maps/api/js?key={{ site.maps_api_key }}&callback=initMap"
async defer></script>