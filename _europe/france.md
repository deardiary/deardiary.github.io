---
layout: default
title: france
permalink: /france/
image: france.svg
---

<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/europe/"></a>
		<h3 class="country-heading">France</h3>
	</div>
</div>



<div class="row">
	
	<ul class="country-stats-container">
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/francepop.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/francecap.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/franceflag.svg"/></li>
	</ul>
	<p class="explanation-text">Posts</p>
	<ul class="post-list country-post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.france limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>