---
layout: page
title: Projects
#featured-image: images/projects-header.jpg
---

<section>
<h3>Featured projects</h3>
<!--<p>Paragraph here.</p>-->
{% include project-tiles.html %}
</section>

<hr />

<section>
<h3>Other projects</h3>
<!--<p>Paragraph here.</p>-->

<div class="box alt">
<div class="row uniform">
    {% for image in site.static_files %}
        {% if image.path contains 'images/projects-gallery' %}
            <div class="4u"><span class="image fit"><a href="{{ image.path }}"><img src="{{ image.path }}" alt="" /></a></span></div>
        {% endif %}
    {% endfor %}
</div>
</div>

<iframe width="310" height="315" src="https://www.youtube-nocookie.com/embed/hSWlU29VHWo?rel=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/BqCQMALBZvQ?rel=0&amp;showinfo=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

</section>
