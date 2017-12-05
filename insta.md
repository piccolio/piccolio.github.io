---
layout: home
title: Antonio Trento
image: assets/images/fulls/my-face.jpg
---
	{% instagram accesstokenpath:/access-token.txt %}
		<div>
			<h3>{{ item.caption.text }}</h3>
			<img src="{{ item.images.standard_resolution.url }}" />
		</div>
	{% endinstagram %}


<!-- Thumbnail -->
<section id="thumbnails">{% for photo in site.photos %}
	<article>
		<a class="thumbnail" href="{{ photo.image }}" data-position="left center"><img src="{{ photo.thumbnail }}" alt="" /></a>
		<h2>{{ photo.title }}</h2>
		<p>{{ photo.caption }}</p>
	</article>
{% endfor %}</section>
