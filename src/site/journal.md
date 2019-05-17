---
title: Reading & Writing
subtitle: Designer | Developer
layout: layouts/page.njk
---

{%- for page in collections.post | reverse -%}
<h2><a href="{{ page.url }}">{{ page.data.title }}</a></h2>
<i class="far fa-calendar-alt"></i> {{ page.date | dateDisplay("LLL d, y") }}
<p>{{ page.data.summary }}</p>
{%- endfor -%}