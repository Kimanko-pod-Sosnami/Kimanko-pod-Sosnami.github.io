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
            <li class="tab is-active" onclick="openTab(event,'Eat')"><a><span class="icon is-small"><i class="fas fa-utensils" aria-hidden="true"></i></span><span>Eat</span></a></li>
            <li class="tab" onclick="openTab(event,'See')"><a><span class="icon is-small"><i class="fas fa-binoculars" aria-hidden="true"></i></span><span>See</span></a></li>
            <li class="tab" onclick="openTab(event,'Kids')"><a><span class="icon is-small"><i class="fas fa-ice-cream" aria-hidden="true"></i></span><span>Kids</span></a></li>
            <li class="tab" onclick="openTab(event,'Sports')"><a><span class="icon is-small"><i class="fas fa-hiking" aria-hidden="true"></i></span><span>Sports</span></a></li>
          </ul>
        </div>
    </nav>
    <div class="container section">
        <div id="Eat" class="content-tab is-active" >
          <div class="content">
<div markdown="1">

  * [Kozia Zagroda](http://www.koziazagroda.com/) - Polish specialties
  * Restauracja Beskid
    * Brenna, Wyzwolenia 89
  * Wędzarnia Kita Wędzona - Butcher with polish specialties. Excellent sausages for the campfire !
    * Brenna, Bukowa 5
  * [Biedronka](https://www.biedronka.pl/) - Supermarket
    * Brenna, Wyzwolenia 38B
    
</div>
          </div>
        </div>
        <div id="See" class="content-tab">
            <div class="content">
              test2<br>
            Details Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</div>
        </div>
        <div id="Kids" class="content-tab">
           <div class="content">
            <ul>
            <li><a href="https://turysta.brenna.org.pl/pl/bajkowy-szlak-utopca">Fairytale Trail of the Utopca</a></li>
            <li><a href="http://www.lesnypark.pl/">Forest Park of Surprises in Ustroń</a></li>
            <li><a href="http://www.parklinowy.pl/">Rope Park on Góra Równica</a></li>
            <li><a href="http://www.chlebowachata.pl/">Chlebowa Chata</a></li>
            <li><a href="http://www.koziazagroda.com/">Goat Farm</a><ul>
            <ul><li>Brenna Centrum, ul. Sportowa 3</li></ul>
            </ul>
            </li>
            <li><a href="https://business.facebook.com/pumptrackbrenna/">Pumptrack</a> - bicycle playground<ul>
            <ul><li>Brenna, ul. Górkacka 224</li></ul>
            </ul>
            </li>
            <li>Recreational square in the Tourism Park<ul>
            <ul><li>Brenna, ul. Malinowa 2b</li>
            <li>Children&#39;s Playground</li>
            <li>miniature golf and floorball</li>
            <li>in winter there is also an ice rink</li></ul>
            </ul>
            </li>
            <li>Hołcyna water harbor<ul>
            <ul><li>about 1.5 km from the center of Brenna</li>
            <li>pedal boat and kayak rental in summer</li></ul>
            </ul>
            </li>
            <li>Hucuł horse riding center<ul>
            <ul><li>Brenna, ul. Jatny 120</li>
            <li>Horse riding lessons on offer, horse walks in the field, one, two and several days horse rides, carriage rides, and in winter - sleigh rides.</li>
            </ul>
            </ul>
            </li>
            </ul>
          </div>
        </div>
        <div id="Sports" class="content-tab">
        <div class="content">
        <ul>
          <li>Hiking trails</li>
          <ul>
            <li>follow the green trail from the center of Brenna to the Błatnia peak, where the PTTK hostel is located.</li>
            <li>follow the yellow trail from Brenna Bukowa to Uncle Tom's Cottage (1h, most of the trail on asphalt)</li>
            <li>follow the black trail to Równica, where the PTTK shelter and rope park are located</li>
            <li>Loop: Brenna - Hołcyna - Kotarz (blue trail) - Grabowa (red trail) - Stary Groń (black trail) - Brenna (further on the black trail, about 16km, we pass the lookout tower between Grabowa and Stary Groń and the Chata Grabowa Hostel</li>
            <li>Loop: Brenna - Błatnia (green trail) - Klimczok (yellow trail) - Uncle Tom's Cottage (red trail) - Brenna Bukowa (yellow trail) about 18km</li>
          </ul>
         <li>For running fans: <a href="http://brenskiekierpce.pl/">http://brenskiekierpce.pl/</a></li>
        </ul> 
        </div>
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

