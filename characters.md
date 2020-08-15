---
layout: blog-layout.liquid
title: Rick & Characters
---

<div class="row">
{% for char in characters %}

<div class="card col-4 col" style="width: 15rem;">
  <img src="{{char.image}}" alt="Card example image">

  <div class="card-body">
    <h4 class="card-title">{{ char.name }}</h4>
    <h5 class="card-subtitle">{{ char.location.name }}</h5>
    <h5 class="card-subtitle">{{ char.gender }}</h5>
    <p class="card-text">Notice that the card width in this example have been set to 20rem, otherwise it will try to fill the current container/row where the card is.</p>
    <a href="/character/{{ char.name|slug}}/" class="paper-btn">Let me go here!</a>
  </div>
</div>

{% endfor %}

</div>
