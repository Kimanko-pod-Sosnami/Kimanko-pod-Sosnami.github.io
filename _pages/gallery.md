---
layout: default
title: Gallery
permalink: /gallery/
---

<h1>Gallery</h1>

<h2>Our guesthouse and the garden</h2>

<div class="gallery">
    <ul id="garden-gallery" class="gallery list-unstyled cS-hidden">
        {% for image in site.data.gallery_garden.images %}
        <li data-thumb="{{ image.thumb_path }}"> 
            <img src="{{ image.path }}" />
            <p>{{ image.description }}</p>
        </li>    
        {% endfor %}
    </ul>
</div>

<br /><br />

<h2>Things to see in Brenna</h2>

<div class="gallery">
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