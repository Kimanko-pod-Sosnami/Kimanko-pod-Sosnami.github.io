---
layout: default
title: Offer
permalink: /offer/
pl_link: /oferta/
---

# Offer


Our guesthouse, "Kimanko pod Sosnami", is located in a quiet and peaceful district in Brenna, walking-distance
from the city center. Ideal for for people who value peace and quiet, nature lovers and families with children. 


<br />
We currently have <strong>three guest rooms</strong> on the second floor. Each room was recently
renovated and comes with a <strong>flat-screen TV</strong>, a <strong>private bathroom</strong> with a sink, toilet and shower. On the same 
floor there is <strong>kitchen</strong> (equipped with a fridge, microwave, water-cooker, mini-stove for preparing breakfast or 
a quick snack) that can be used by guests and a <strong>kids corner</strong> with toys, color books, ... perfect during
rainy days.


<br />
The <strong>large garden</strong> surrounding the guesthouse is available for guests. There are 
<strong>picnic benches</strong> and a spot for <strong>campfires</strong>.
Check out our [gallery]({{ site.baseurl }}/gallery/)!

<br />
<div class="card">
  <header class="card-header">
    <nav class="tabs is-medium">
        <ul>
          <li id="r1-tab" class="tab"><a><span>Room 1</span></a></li>
          <li id="r2-tab" class="tab is-active"><a><span>Room 2</span></a></li>
          <li id="r3-tab" class="tab"><a><span>Room 3</span></a></li>
          <li id="r4-tab" class="tab"><a><span>Room 4</span></a></li>
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
