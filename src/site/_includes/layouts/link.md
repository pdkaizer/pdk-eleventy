---
layout: layouts/base.njk
pageClass: posts
templateEngineOverride: njk, md
---

{% include "header-image.njk" %}

<p class="date">
  Posted as an example, on <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
</main>


<div class="page-area">
	<section class="article-area">
		<article itemscope itemtype="http://schema.org/BlogPosting">
			<div class="post-content" itemprop="articleBody">
			<h1 itemprop="name headline">{{ page.title }}</h1>
			<span class="visible-phone mobile-date">
				<time datetime="{{ page.date | date_to_xmlschema }}" itemprop="datePublished"><i class="far fa-calendar-alt"></i> {{ page.date | date: "%b %-d, %Y" }}</time>
			</span>
	    	<div class="post-meta visible-desktop">
	    		<time datetime="{{ page.date | date_to_xmlschema }}" itemprop="datePublished"><i class="far fa-calendar-alt"></i> {{ page.date | date: "%b %-d, %Y" }}</time>
	    	</div>
	    	 {{ content | safe }}
			</div>
		</article>
		{% include "coments.njk" %}
	</section>
</div>

