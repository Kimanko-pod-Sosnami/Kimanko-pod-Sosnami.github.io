---
layout: default
title: Contact
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
<br />
<div class="card">
    <nav class="tabs is-centered is-medium">
        <div class="container">
          <ul>
            <li class="tab is-active" onclick="openTab(event,'Car')"><a><span class="icon is-small"><i class="fas fa-car" aria-hidden="true"></i></span><span>by Car</span></a></li>
            <li class="tab" onclick="openTab(event,'Bus')"><a><span class="icon is-small"><i class="fas fa-bus-alt" aria-hidden="true"></i></span><span>by Bus</span></a></li>
            <li class="tab" onclick="openTab(event,'Train')"><a><span class="icon is-small"><i class="fas fa-train" aria-hidden="true"></i></span><span>by Train</span></a></li>
            <li class="tab" onclick="openTab(event,'Plane')"><a><span class="icon is-small"><i class="fas fa-plane-departure" aria-hidden="true"></i></span><span>by Plane</span></a></li>
          </ul>
        </div>
    </nav>
    
    <div class="container section">
        <div id="Car" class="content-tab is-active" >
          <p>
            test1<br>
          Overview Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="Bus" class="content-tab">
            <p>
              test2<br>
            Details Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="Train" class="content-tab">
           <p>
             test3 <br>  
           Specification Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="Plane" class="content-tab">
           <p>
             test3 <br>  
           Specification Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
    </div>
</div>

<div class="section">
</div>
<div class="section">
</div>

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

    var styles = {
      default: null,
      hide: [
        {
          featureType: 'poi.business',
          stylers: [{visibility: 'off'}]
        },
        {
          featureType: 'transit',
          elementType: 'labels.icon',
          stylers: [{visibility: 'off'}]
        }
      ]
    };

    addMarker({
        coords: {lat: 49.7186637, lng: 18.9394271},
    });

    map.setOptions({styles: styles['hide']});

  }
    
</script>
<script src="https://maps.googleapis.com/maps/api/js?key={{ site.maps_api_key }}&callback=initMap"
async defer></script>