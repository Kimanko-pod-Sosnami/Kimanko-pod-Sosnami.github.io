---
layout: default.pl
title: Oferta
permalink: /oferta/
---

# Oferta


Do Państwa dyspozycji oddajemy trzy świeżo wyremontowane pokoje z nowymi łazienkami oraz ogromny ogród z placem zabaw 
i miejscem na ognisko. W domu znajduje sie również mały pokój zwany bawialnią, który udostępniony jest jako miejsce 
zabawy dla najmłodszych. Do Państwa dyspozycji jest tez  w pełni wyposażona kuchnia. Miejsce to szczególnie polecane 
jest osobom ceniącym ciszę, miłośnikom przyrody oraz rodzinom z dziećmi. Szczegółowy opis w zakładce 
[galeria]({{ site.baseurl }}/galeria/).

<br />
<div class="card">
  <header class="card-header">
    <nav class="tabs is-medium">
        <ul>
          <li id="r1-tab" class="tab"><a><span>Pokój 1</span></a></li>
          <li id="r2-tab" class="tab is-active"><a><span>Pokój 2</span></a></li>
          <li id="r3-tab" class="tab"><a><span>Pokój 3</span></a></li>
          <li id="r4-tab" class="tab"><a><span>Pokój 4</span></a></li>
        </ul>
    </nav> 
  </header>
    <div id="R1" class="content-tab">
        <div class="columns">
            <div class="column is-12">
                <div class="card-content">Room 1 on the ground floor is currently being 
                renovated an is not available for guests.</div>
            </div> 
        </div>
    </div>
    <div id="R2" class="content-tab is-active">
        <div class="columns">
            <div class="column is-6">
                <div class="card-content">
                A double room with a double bed, wardrobe, table with chairs, flat TV 
                and bathroom.
                <br /><br /><br /><br />
                
                The rate for this room starts from <strong>PLN {{ site.data.prices.double_room }}</strong> (per night)
                
                </div>
            </div>    
            <div class="column is-6">
            <ul id="gallery-room2" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room2.images %}
                <li data-thumb="{{ site.baseurl }}{{ image.thumb_path }}"> 
                    <img src="{{ site.baseurl }}{{ image.path }}" />
                    <p>{{ image.description }}</p>
                </li>    
                {% endfor %}
            </ul>
            </div>
        </div>
    </div>
    <div id="R3" class="content-tab">
        <div class="columns">
            <div class="column is-6">
                <div class="card-content">Room for 2-4 people with one large bed and fold-out sofa, wardrobe, 
                small table, TV and a new bathroom (shower with extra deep tub, useful for bathing small children). 
                Recommended for people who prefer more space or parents with their children.
                                <br /><br /><br /><br />
                
                The rate for this room starts from <strong>PLN {{ site.data.prices.large_room }}</strong> (per night)
                </div>
            </div>    
            <div class="column is-6">              
            <ul id="gallery-room3" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room3.images %}
                <li data-thumb="{{ site.baseurl }}{{ image.thumb_path }}"> 
                    <img src="{{ site.baseurl }}{{ image.path }}" />
                    <p>{{ image.description }}</p>
                </li>    
                {% endfor %}
            </ul>
            </div> 
        </div>
    </div>
    <div id="R4" class="content-tab">
        <div class="columns">
            <div class="column is-6">
                <div class="card-content">Double room with two single beds (can be joined), wardrobe, table with 
                chairs, bathroom and flat-screen TV.
                                <br /><br /><br /><br />
                
                The rate for this room starts from <strong>PLN {{ site.data.prices.double_room }}</strong> (per night)
                </div>
            </div>    
            <div class="column is-6">
            <ul id="gallery-room4" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room4.images %}
                <li data-thumb="{{ site.baseurl }}{{ image.thumb_path }}"> 
                    <img src="{{ site.baseurl }}{{ image.path }}" />
                    <p>{{ image.description }}</p>
                </li>    
                {% endfor %}
            </ul>
            </div>
        </div>
  </div>
  <footer class="card-footer">
    <a href="{{ site.baseurl }}/prices/" class="card-footer-item">Rates &amp; Reservations</a>
  </footer>
</div>

<div class="section">
</div>
<script>
    $(document).ready(function() {
            function init_gallery(gallery) {
                return $(gallery).lightSlider({
                    gallery:true,
                    item:1,
                    thumbItem:9,
                    slideMargin: 0,
                    speed:500,
                    auto:false,
                    //loop:true,
                    onSliderLoad: function() {
                        $(gallery).removeClass('cS-hidden');
                    }  
                });            
            }
    
            //init default gallery
            init_gallery('#gallery-room2');
            init_gallery('#gallery-room3');
            init_gallery('#gallery-room4');
            
            $('#r1-tab').click(function(ev) {
                openTab(ev,'R1');
            });            
            $('#r2-tab').click(function(ev) {
                openTab(ev,'R2');
            });
            $('#r3-tab').click(function(ev) {
                openTab(ev,'R3');
            });
            $('#r4-tab').click(function(ev) {
                openTab(ev,'R4');
            });
    });
</script>
