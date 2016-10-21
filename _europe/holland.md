---
layout: default
title: holland
permalink: /holland/
image: holland.png
---

<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/europe/"></a>
	</div>
</div>

<div class="row">
	<h3 class="country-heading">Holland</h3>
	<ul class="post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.holland limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>