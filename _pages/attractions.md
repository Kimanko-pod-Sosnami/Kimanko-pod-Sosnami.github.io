---
layout: default
title: Attractions
permalink: /attractions/
pl_link: /atrakcje/
---

# Attractions

The center of [Brenna](https://en.wikipedia.org/wiki/Brenna,_Poland) is within walking distance of our guesthouse,
here you'll find various restaurants and shops. It is worth noting that in the vicinity there is a local butcher who 
prepares delicious sausages (perfect for roasting above a fire!) and other home-made products (about 800m). For people looking for a more active holiday, there are hiking trails 
starting from Brenna, while those travelling with children will be happy to find playground and activities for 
kids nearby. The river Brennica is within walking distance (350m), where you can relax by the water.

<br />
<div class="card">
    <nav class="tabs is-centered is-medium">
        <div class="container">
          <ul>
            <li class="tab is-active" onclick="openTab(event,'Eat')"><a><span class="icon is-small"><i class="fas fa-utensils" aria-hidden="true"></i></span><span>Eat</span></a></li>
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
        <div id="Kids" class="content-tab">
           <div class="content">
<div markdown="1">
  * [Fairytale Trail of the Utopca](https://turysta.brenna.org.pl/pl/bajkowy-szlak-utopca)
  * [Forest Park of Surprises in Ustroń](http://www.lesnypark.pl/)
  * [Rope Park on Góra Równica](http://www.parklinowy.pl/)
  * [Chlebowa Chata](http://www.chlebowachata.pl/)
  * [Kozia Zagroda](http://www.koziazagroda.com/) Goat Farm and restaurant
    * Brenna Centrum, ul. Sportowa 3
  * [Pumptrack](https://business.facebook.com/pumptrackbrenna/) - bicycle playground
    * Brenna, ul. Górkacka 224
  * Recreational square in the Tourism Park
    * Brenna, ul. Malinowa 2b
    * Children's Playground
    * Miniature golf and floorball
    * Ice rink (winter only)
  * [Przystań Wodna Brenna Hołcyna](https://www.facebook.com/pages/category/Rental-Shop/Przysta%C5%84-Wodna-Brenna-Ho%C5%82cyna-798352830292770/) - Brenna's "harbor" pedal boat and kayak rental
    * Only in summer
    * About 1.5 km from the center
  * Hucuł horse riding center
    * Brenna, ul. Jatny 120
    * Horse riding lessons
    * Horse walks in the field
    * One, two and several days horse ride trips
    * carriage rides, and in winter - sleigh rides.
            
  
</div>
          </div>
        </div>
        <div id="Sports" class="content-tab">
        <div class="content">
<div markdown="1">

  * Hiking trails
    * follow the green trail from the center of Brenna to the **Błatnia** peak, where the PTTK hostel is located.
    * follow the black trail to **Równica**, where the PTTK shelter and rope park are located
    * Loop: Brenna - Hołcyna - **Kotarz** (blue trail) - Grabowa (red trail) - **Stary Groń** (black trail) - Brenna (further on the black trail, about 16km, we pass the lookout tower between Grabowa and Stary Groń and the Chata Grabowa Hostel
    * Loop: Brenna - **Błatnia** (green trail) - **Klimczok** (yellow trail) - Uncle Tom's Cottage (red trail) - Brenna Bukowa (yellow trail) about 18km
  * For running fans: [http://brenskiekierpce.pl/](http://brenskiekierpce.pl/)
  * [Pumptrack](https://business.facebook.com/pumptrackbrenna/) - bicycle playground
    * Brenna, ul. Górkacka 224
  * Recreational square in the Tourism Park
    * Brenna, ul. Malinowa 2b
    * Miniature golf and floorball
    * Ice rink (winter only)
  * [Przystań Wodna Brenna Hołcyna](https://www.facebook.com/pages/category/Rental-Shop/Przysta%C5%84-Wodna-Brenna-Ho%C5%82cyna-798352830292770/) - Brenna's "harbor" pedal boat and kayak rental
    * Only in summer
    * About 1.5 km from the center
  * Hucuł horse riding center
    * Brenna, ul. Jatny 120
    * Horse riding lessons
    * Horse walks in the field
    * One, two and several days horse ride trips
    * carriage rides, and in winter - sleigh rides.
</div>
        </div>
        </div>
    </div>
    <!--<div id="map"></div>-->
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

