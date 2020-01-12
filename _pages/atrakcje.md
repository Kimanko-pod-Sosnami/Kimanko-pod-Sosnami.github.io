---
layout: default.pl
title: Atrakcje
permalink: /atrakcje/
en_link: /attractions/
---

# Atrakcje

Dom oddalony jest od centrum [Brennej](https://en.wikipedia.org/wiki/Brenna,_Poland) około 20-minutowym spacerem Do 
rzeki Brennicy jest bardzo blisko około 350 m, gdzie można zrelaksować sie nad wodą w ciepłe, letnie dni. W centrum 
Brennej znajduje się Biedronka oraz kilka innych sklepów, gdzie znajdą Państwo wszystkie potrzebne produkty. Warto 
dodać, że w niedalekiej okolicy znajduje się wędzarnia z pysznymi kiełbaskami (idealne na ognisko!) oraz innymi 
swojskimi wyrobami (ok 800m). W okolicy znajduje się sporo atrakcji dla dzieci oraz osób lubiących aktywnie spędzać 
czas.

<br />
<div class="card">
    <nav class="tabs is-centered is-medium">
        <div class="container">
          <ul>
            <li class="tab is-active" onclick="openTab(event,'Eat')"><a><span class="icon is-small"><i class="fas fa-utensils" aria-hidden="true"></i></span><span>Restauracje</span></a></li>
            <li class="tab" onclick="openTab(event,'Kids')"><a><span class="icon is-small"><i class="fas fa-ice-cream" aria-hidden="true"></i></span><span>Dzieci</span></a></li>
            <li class="tab" onclick="openTab(event,'Sports')"><a><span class="icon is-small"><i class="fas fa-hiking" aria-hidden="true"></i></span><span>Sport</span></a></li>
          </ul>
        </div>
    </nav>
    <div class="container section">
        <div id="Eat" class="content-tab is-active" >
          <div class="content">
<div markdown="1">

  * [Kozia Zagroda](http://www.koziazagroda.com/)
  * Restauracja Beskid
    * Brenna, Wyzwolenia 89
  * Wędzarnia Kita Wędzona
    * Brenna, Bukowa 5
    
</div>
          </div>
        </div>
        <div id="Kids" class="content-tab">
           <div class="content">
<div markdown="1">
  * [Bajkowy Szlak Utopca](https://turysta.brenna.org.pl/pl/bajkowy-szlak-utopca)
  * [Leśny Park Niespodzianek](http://www.lesnypark.pl/)
  * [Park Linowy na Górze Równica](http://www.parklinowy.pl/)
  * [Chlebowa Chata](http://www.chlebowachata.pl/)
  * [Kozia Zagroda](http://www.koziazagroda.com/)
    * Brenna Centrum, ul. Sportowa 3
  * [Pumptrack](https://business.facebook.com/pumptrackbrenna/) - rowerowy plac zabaw 
    * Brenna, ul. Górkacka 224
  * Rekreacyjny plac w Parku Turystyki
    * Brenna, ul. Malinowa 2b
    * plac zabaw dla dzieci
    * minigolf oraz unihokej
    * w zimę znajduje się tu również lodowisko
  * [Przystań wodna Hołcyna](https://www.facebook.com/pages/category/Rental-Shop/Przysta%C5%84-Wodna-Brenna-Ho%C5%82cyna-798352830292770/)
    * ok 1.5km od centrum Brennej, możliwość wynajęcia rowerków wodnych oraz kajaków w okresie letnim
  * Ośrodek jazdy konnej Hucuł
    * Brenna, ul. Jatny 120
    * W ofercie nauka jazdy konnej, spacery konne w terenie, rajdy konne jedno, dwu i kilku dniowe, przejażdżki bryczkami, a w zimie – kuligi.
            
  
</div>
          </div>
        </div>
        <div id="Sports" class="content-tab">
        <div class="content">
<div markdown="1">

  * Wycieczki w góry
    * szlakiem zielonym z centrum Brennej na szczyt Błatnia, gdzie znajduje się schronisko PTTK 
    * szlakiem żółtym z Brennej Bukowej do Chaty Wuja Toma (1godz, większość szlaku asfaltem)
    * szlakiem czarnym na Równicę, gdzie znajduje się schronisko PTTK oraz park linowy
    * pętla: Brenna - Hołcyna  -  Kotarz (szlak niebieski) - Grabowa (szlak czerwony)  - Stary Groń (szlak czarny) - Brenna (dalej szlak czarny, ok 16km, mijamy wieżę widokowa pomiędzy Grabową a Starym Groniem oraz Schronisko Chata Grabowa
    * pętla: Brenna – Błatnia (szlak zielony) – Klimczok (szlak żółty) – Chata Wuja Toma (szlak czerwony) – Brenna Bukowa (szlak żółty) ok 18km
  * Dla fanów biegania [http://brenskiekierpce.pl/](http://brenskiekierpce.pl/)
  * [Pumptrack](https://business.facebook.com/pumptrackbrenna/) - rowerowy plac zabaw 
    * Brenna, ul. Górkacka 224
  * Rekreacyjny plac w Parku Turystyki
    * Brenna, ul. Malinowa 2b
    * minigolf oraz unihokej
    * w zimę znajduje się tu również lodowisko
  * [Przystań wodna Hołcyna](https://www.facebook.com/pages/category/Rental-Shop/Przysta%C5%84-Wodna-Brenna-Ho%C5%82cyna-798352830292770/)
    * ok 1.5km od centrum Brennej, możliwość wynajęcia rowerków wodnych oraz kajaków w okresie letnim
  * Ośrodek jazdy konnej Hucuł
    * Brenna, ul. Jatny 120
    * W ofercie nauka jazdy konnej, spacery konne w terenie, rajdy konne jedno, dwu i kilku dniowe, przejażdżki bryczkami, a w zimie – kuligi.
         
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

