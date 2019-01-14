---
layout: page
title: 技术分享
description: 博观而约取，厚积而薄发
image: assets/images/people.jpg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">
	<section id="one">
		<div class="inner">
			<header class="major">
				<h1>{{ page.title }}</h1>
			</header>
			<div class="row">
				{% for post in site.posts %}
	  		{% if post.category == 'technology' %}
				<div class="6u 12u$(small)">
					<h3>{{post.title}}</h3>
					<p>{{ post.excerpt }}</p>
					<ul class="actions">
						<li><a href="{{ post.url | relative_url }}" class="button">了解更多</a></li>
					</ul>
				</div>
			  {% endif %}
	  		{% endfor %}
			</div>
		</div>
	</section>
</div>>