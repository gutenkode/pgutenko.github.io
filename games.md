---
layout: page
title: Games
#featured-image: images/games-header.jpg
---

<section>
<!--<p>A collection of my best projects</p>-->
{% include game-tiles.html %}
</section>

<hr />

<section>
<h3>Gallery</h3>
<p>Everything else worth showing</p>

<div class="box alt">
<div height='100' class="row uniform">
    {% assign items = site.static_files | sort: 'name' | reverse %}
    {% for image in items %}
        {% if image.path contains 'images/games-gallery' %}
            <div class="4u"><span class="image fit"><a href="{{ image.path }}"><img src="{{ image.path }}" alt="" /></a></span></div>
        {% endif %}
    {% endfor %}
</div>
</div>
</section>

<p>Anything catch your eye? Want more details? Just feel like saying hello? Send me a message!</p>
