---
layout: layouts/base.njk
title: Photos from my travels
header-image: london-2007-02.jpg
photosets:
	- Malawi:
	- Maine:
---

<div class="page-area">

<h1>Photosets from my travels</h1>

<ul class="photos-grid">
	{%- for photoset in tag.photosets -%}
	<li>
		<a href="{{ photoset.url }}">
		<img src="/images/photos/{{photoset.photoset-name}}/{{photoset.featured-image}}.jpg" class="img-responsive" alt="{{photoset.photosetname}}">
		<h3>{{ photoset.title }}</h3>
		</a>
	</li>
	{% endfor %}
</ul>

</div>