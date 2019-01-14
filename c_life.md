---
title: 生活点滴
layout: landing
description: 我感激我们的光锥曾彼此重叠，而你永远改变了我的星轨
image: assets/images/pic07.png
nav-menu: true
---

<!-- Main -->
<div id="main">
	<section id="two" class="spotlights">
	  {% for post in site.posts %}
	  {% if post.category == 'life' %}
			<section>
				<a href="{{ post.url | relative_url  }}"  class="image">
					<img src="{{ post.image }}"  alt="" data-position="center center" />
				</a>
				<div class="content">
					<div class="inner">
						<header class="major">
							<h3>{{post.title}}</h3>
						</header>
						<p>{{ post.excerpt }}</p>
						<ul class="actions">
							<li><a href="{{ post.url | relative_url  }}"  class="button">了解更多</a></li>
						</ul>
					</div>
				</div>
			</section>
	  {% endif %}
	  {% endfor %}
	</section>
</div>
