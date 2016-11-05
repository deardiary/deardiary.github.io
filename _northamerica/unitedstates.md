---
layout: default
title: United States of America
permalink: /unitedstates/
image: usa.svg
---
<div class="row">
	<div class="country-header">
		<a class="back-explore glyphicon glyphicon-chevron-left" href="{{site.baseurl}}/continents/northamerica/"></a>
		<h3 class="country-heading">United States Of America</h3>
	</div>
</div>


<div class="">
	
	<ul class="country-stats-container">
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/usapop.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/usacap.svg"/></li>
		<li class=""><img class="" src="{{site.baseurl}}/assets/countries/usaflag.svg"/></li>
	</ul>
	<p class="explanation-text">Posts</p>
	<ul class="post-list country-post-list col-md-8 col-md-offset-2">
		{% for post in site.categories.usa limit:10 %}
			<li class='single-post'>
			    <h2><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a></h2>
				<span class="post-meta col-xs-12">{{ post.date | date: "%b %-d, %Y" }}</span>
				<span class="post-excerpt">{{ post.excerpt }} </span><a class="post-end-link" href="{{ post.url | prepend: site.baseurl }}"> Read on...</a>
			 </li>
		{% endfor %}
	</ul>
</div>