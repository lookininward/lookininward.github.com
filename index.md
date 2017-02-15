---
layout: page
title: lookininward
tagline: a place for my thoughts
---
{% include JB/setup %}

{% for post in site.posts limit:3 %}
<div class="panel panel-default">
	<div class="panel-heading">
		{{ post.date | date_to_string }} 
		<a href="{{ BASE_PATH}}{{ post.url }}">{{ post.title }}</a>
	</div>
	<div class="panel-body">
		{{ post.content }}
	</div>
</div>
{% endfor %}
