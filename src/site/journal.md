---
title: Peter Kaizer
subtitle: Designer | Developer
layout: layouts/base.njk
---

<div class="page-area">

<section class="article-area">

  # Reading & Writing

{%- for page in collections.post | reverse -%}
<h2><a href="{{ page.url }}">{{ page.data.title }}</a></h2>
<i class="far fa-calendar-alt"></i> {{ page.date | dateDisplay("LLL d, y") }}
<p>{{ page.data.summary }}</p>
{%- endfor -%}

</section>

</div>