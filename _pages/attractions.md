---
layout: default
title: Attractions
permalink: /attractions/
---

# Attractions

The center of [Brenna](https://en.wikipedia.org/wiki/Brenna,_Poland) is within walking distance of our guesthouse,
here you'll find various restaurants and shops. For people looking for a more active holiday, there are hiking trails 
starting from Brenna, while those travelling with children will be happy to find playground and activities for 
kids nearby. 

<br />
<div class="card">
    <nav class="tabs is-centered is-medium">
        <div class="container">
          <ul>
            <li class="tab is-active" onclick="openTab(event,'Eat')"><a><span class="icon is-small"><i class="fas fa-utensils" aria-hidden="true"></i></span><span class="is-hidden-mobile">Eat</span></a></li>
            <li class="tab" onclick="openTab(event,'See')"><a><span class="icon is-small"><i class="fas fa-binoculars" aria-hidden="true"></i></span><span class="is-hidden-mobile">See</span></a></li>
            <li class="tab" onclick="openTab(event,'Kids')"><a><span class="icon is-small"><i class="fas fa-ice-cream" aria-hidden="true"></i></span><span class="is-hidden-mobile">Kids</span></a></li>
            <li class="tab" onclick="openTab(event,'Sports')"><a><span class="icon is-small"><i class="fas fa-hiking" aria-hidden="true"></i></span><span class="is-hidden-mobile">Sports</span></a></li>
          </ul>
        </div>
    </nav>
    
    <div class="container section">
        <div id="Eat" class="content-tab is-active" >
          <p>
            test1<br>
          Overview Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="See" class="content-tab">
            <p>
              test2<br>
            Details Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="Kids" class="content-tab">
           <p>
             test3 <br>  
           Specification Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
        <div id="Sports" class="content-tab">
           <p>
             test3 <br>  
           Specification Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
        </div>
    </div>
    <div id="map"></div>
</div>




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

