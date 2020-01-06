---
title: Peter Kaizer
subtitle: Designer | Developer
layout: layouts/base.njk
headerImage: DC-2019-fall.jpg
pagination:
  data: collections.post
  size: 6
  reverse: true
---
{% include "home-hero.njk" %}
{% include "home-header-image-down.njk" %}

<section class="posts" id="follow">

<h1><i class="fal fa-pencil"></i> Latest reading & writing</h1>
{% include "home-posts-listing.njk" %}
<div class="home-see-all"><h3><a href="/journal">See all posts <i class="fa fa-arrow-right fa=2x" aria-hidden="true"></i></a></h3></div>
</section>

{% include "home-featured-project.njk" %}

{% include "home-featured-photo-gallery.njk" %}