---
layout: default
title: Kimanko pod Sosnami - Gallery
permalink: /gallery/
---

<h1>Gallery</h1>

<h2>Our Bed & Breakfast and the Garden</h2>

<ul id="garden-gallery" class="gallery list-unstyled cS-hidden">
    {% for image in site.data.gallery_garden.images %}
    <li data-thumb="{{ image.thumb_path }}"> 
        <img src="{{ image.path }}" />
        <p>{{ image.description }}</p>
    </li>    
    {% endfor %}
</ul>

<div class="section">
<h2>Things to see in Brenna</h2>

<ul id="brenna-gallery" class="gallery list-unstyled cS-hidden">
    {% for image in site.data.gallery_brenna.images %}
    <li data-thumb="{{ image.thumb_path }}"> 
        <img src="{{ image.path }}" />
        <p>{{ image.description }}</p>
    </li>    
    {% endfor %}
</ul>
</div>

<script type="text/javascript">
    $(document).ready(function() {
            $('#garden-gallery').lightSlider({
                gallery:true,
                item:1,
                thumbItem:9,
                slideMargin: 0,
                speed:500,
                auto:false,
                loop:true,
                onSliderLoad: function() {
                    $('#garden-gallery').removeClass('cS-hidden');
                }  
            });
            $('#brenna-gallery').lightSlider({
                gallery:true,
                item:1,
                thumbItem:9,
                slideMargin: 0,
                speed:500,
                auto:false,
                loop:true,
                onSliderLoad: function() {
                    $('#brenna-gallery').removeClass('cS-hidden');
                }  
            });
    });
</script>