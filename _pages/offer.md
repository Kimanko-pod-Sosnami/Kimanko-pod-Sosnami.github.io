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
    <p class="card-header-title">
      Our Rooms
    </p>
    <nav class="tabs is-medium">
        <ul>
          <li class="tab" onclick="openTab(event,'R1')"><a><span>Room 1</span></a></li>
          <li class="tab is-active" onclick="openTab(event,'R2')"><a><span>Room 2</span></a></li>
          <li class="tab" onclick="openTab(event,'R3')"><a><span>Room 3</span></a></li>
          <li class="tab" onclick="openTab(event,'R4')"><a><span>Room 4</span></a></li>
        </ul>
    </nav> 
  </header>
  <div class="card-content">
    <div class="container section">
        <div id="R1" class="content-tab" style="display:none">
          <p>Under renovation</p>  
        </div>
        <div id="R2" class="content-tab">
            <div class="columns">
                <div class="column is-8">Description here</div>
                <div class="column is-4">Gallery here</div>
            </div>
        </div>
        <div id="R3" class="content-tab" style="display:none">
            <div class="columns">
                <div class="column is-8">Description here</div>
                <div class="column is-4">Gallery here</div>
            </div>
        </div>
        <div id="R4" class="content-tab" style="display:none">
            <div class="columns">
                <div class="column is-8">Description here</div>
                <div class="column is-4">Gallery here</div>
            </div>
        </div>
    </div>
  </div>
  <footer class="card-footer">
    <a href="{{ site.baseurl }}/prices/" class="card-footer-item">Prices</a>
    <a href="{{ site.baseurl }}/reservations/" class="card-footer-item">Reservations</a>
  </footer>
</div>