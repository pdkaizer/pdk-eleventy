---
title: Peter Kaizer
subtitle: Designer | Developer
layout: layouts/base.njk
---

<div class="page-area">

  <article class="home-main">

  ## Hi there, I am Peter Kaizer

I am a designer & developer with a passion for user focused digital products that are highly functional and beautifully designed.

My current job is Senior Designer for <a href="http://www.boozallen.com/">Booz | Allen | Hamilton</a> where I currently am doing design work for the <a href="https://www.usps.com/">USPS</a>.

This is my personal web space, where I post about technology, design and food, along with other things that catch my eye.  You can read more <a href="/about">about me</a> or <a href="/contact">contact me</a>

Also check out my <a href="http://books.peterkaizer.com/">recommended books site</a>.

  </article>

  <section class ="home-article-listing" id="follow">

  # Latest reading & writing

{%- for page in collections.post -%}

  <h2><a href="{{ page.url }}">{{ page.data.title }}</a></h2>
  <i class="far fa-calendar-alt"></i> {{ page.date | dateDisplay("LLL d, y") }}

{%- endfor -%}

</section>

</div>

