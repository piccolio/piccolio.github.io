---
layout: home
title: Antonio Trento
image: assets/images/fulls/my-face.jpg
---
<script type="text/javascript">
    var feed = new Instafeed({
        get: 'tagged',
        tagName: 'posero',
        clientId: '1093675496.1677ed0.865e98386e4245d4919c25426e03e821'
    });
    feed.run();
</script>
<!-- Thumbnail -->
<section id="thumbnails">{% for photo in site.photos %}
	<article>
		<a class="thumbnail" href="{{ photo.image }}" data-position="left center"><img src="{{ photo.thumbnail }}" alt="" /></a>
		<h2>{{ photo.title }}</h2>
		<p>{{ photo.caption }}</p>
	</article>
{% endfor %}</section>
