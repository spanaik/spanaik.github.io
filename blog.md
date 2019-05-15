---
layout: default
title: Blog
---
<main class="blogs-section">
	<section class="blog-container">
		<h2 class="highlight-bottom">Latest Posts</h2>
		  <div class="blog">
		  {% for post in site.posts %}
		    	<div class="blog-excerpt">
		    		<div class="img-container">{{ post.excerpt }}</div>
		    		<div class="text-container">
			    		<h5>{{ post.category }}</h5>
			    		<h6>{{ post.date | date_to_string }}</h6>
			      		<h4 class="blog-link"><a href="{{ post.url }}">{{ post.title }}</a></h4>
		      		</div>
		      	</div>
		  {% endfor %}
		</div>
	</section>
</main>