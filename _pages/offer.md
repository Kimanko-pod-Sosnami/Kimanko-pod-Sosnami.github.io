---
layout: default
title: Offer
permalink: /offer/
---

# Offer

We currently have three guest rooms on the second floor. Each room was recently
renovated and comes with a TV, a private bathroom equipped with a sink, toilet and shower. On the same floor there is a common
kitchen with equipment that can be used by guests and a kids corner with toys, color books, ...

Room 1 on the ground floor is currently being renovated an is not available for guests. 

<br />
The large garden surrounding the guesthouse is available for guests. There are picnic benches and a spot for campfires.
Visit the [gallery]({{ site.baseurl }}/gallery/) for pictures of the garden.


<br />
<div class="card">
  <header class="card-header">
    <p class="card-header-title is-hidden-mobile">
      Our Rooms
    </p>
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
            <div class="column is-6">
                <div class="card-content">Description here</div>
            </div>
            <div class="column is-6">
                <div class="card-content">Coming soon</div>
            </div> 
        </div>
    </div>
    <div id="R2" class="content-tab is-active">
        <div class="columns">
            <div class="column is-6">
                <div class="card-content">Description here</div>
            </div>    
            <div class="column is-6">
            <ul id="gallery-room2" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room2.images %}
                <li data-thumb="{{ image.thumb_path }}"> 
                    <img src="{{ image.path }}" />
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
                <div class="card-content">Description here</div>
            </div>    
            <div class="column is-6">              
            <ul id="gallery-room3" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room3.images %}
                <li data-thumb="{{ image.thumb_path }}"> 
                    <img src="{{ image.path }}" />
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
                <div class="card-content">Description here</div>
            </div>    
            <div class="column is-6">
            <ul id="gallery-room4" class="gallery list-unstyled cS-hidden">
                {% for image in site.data.gallery_room4.images %}
                <li data-thumb="{{ image.thumb_path }}"> 
                    <img src="{{ image.path }}" />
                    <p>{{ image.description }}</p>
                </li>    
                {% endfor %}
            </ul>
            </div>
        </div>
  </div>
  <footer class="card-footer">
    <a href="{{ site.baseurl }}/prices/" class="card-footer-item">Prices</a>
    <a href="{{ site.baseurl }}/reservations/" class="card-footer-item">Reservations</a>
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
                    loop:true,
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
