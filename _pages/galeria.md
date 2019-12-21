---
layout: default.pl
title: Galeria
permalink: /galeria/
---

<h1>Galeria</h1>

<div id="gallery-page" class="columns is-multiline animated fadein">
{% for image in site.data.gallery.images %}
<div class="column is-3-desktop is-4-tablet is-half-mobile">
<div class="gallery-item">
<a href="{{ site.baseurl }}{{ image.path }}" class="gallery-link" data-sub-html="{{ image.description }}"><img src="{{ site.baseurl }}{{ image.thumb_path }}" data-src="{{ site.baseurl }}{{ image.path }}"/></a>
</div>
</div>
{% endfor %}
</div>

<script type="text/javascript">
    $(document).ready(function() {
        $("#gallery-page").lightGallery({
           thumbnail:true,
           selector: '.gallery-link'
        }); 
    });
</script>