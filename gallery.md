---
layout: page
title: Gallery
#featured-image: images/gallery-header.jpg
---

<p>A collection of projects worth showing</p>

<section>
<div class="box alt">
<div class="row uniform">
    {% assign items = site.static_files | sort: 'name' | reverse %}
    {% for image in items %}
        {% if image.path contains 'images/gallery-photos' %}
            <div class="4u"><span class="image fit"><a href="{{ image.path }}"><img src="{{ image.path }}" alt="" /></a></span></div>
        {% endif %}
    {% endfor %}
</div>
</div>

<iframe width="500" height="315" src="https://www.youtube-nocookie.com/embed/uCRMnpRYdkg?rel=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="500" height="315" src="https://www.youtube-nocookie.com/embed/4J5Ygi6T49w?rel=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

</section>
