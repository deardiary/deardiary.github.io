---
layout: default
title: ireland
permalink: /ireland/
image: ireland.svg
---

<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/europe/"></a>
		<h3 class="country-heading">Ireland</h3>
	</div>
</div>

<div class="">
	<ul class="country-stats-container">
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/irelandpop.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/irelandcap.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/irelandflag.svg"/></li>
	</ul>
	<ul class="post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.ireland limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta col-xs-12">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>