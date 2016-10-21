---
layout: page
title: england
permalink: /england/
image: england.png
---
<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/europe/"></a>
		<h3 class="country-heading">England</h3>
	</div>
</div>

<div class="row">
	<ul class="country-stats-container">
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/englandpop.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/englandcap.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/englandflag.svg"/></li>
	</ul>
	<ul class="post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.england limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>