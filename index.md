---
layout: home
title: Lens by HTML5 UP
---

<!-- Thumbnail -->
<section id="thumbnails">{% for photo in site.photos %}
	<article>
		<a class="thumbnail" href="{{ photo.image }}" data-position="{{ photo.background.position | default: "left center" }}" data-size="{{ photo.background.size | default: "cover" }}"><img src="{{ photo.thumbnail }}" alt="" /></a>
		<h2>{{ photo.title }}</h2>
		<p>{{ photo.caption }}</p>
	</article>
{% endfor %}</section>
