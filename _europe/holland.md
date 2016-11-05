---
layout: default
title: holland
permalink: /holland/
image: holland.svg
---

<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/europe/"></a>
		<h3 class="country-heading">Holland</h3>
	</div>
</div>

<div class="">
	<ul class="country-stats-container">
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/hollandpop.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/hollandcap.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/hollandflag.svg"/></li>
	</ul>
	<ul class="post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.holland limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta col-xs-12">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>