---
layout: page
title: lookininward
tagline: a place for my thoughts
---
{% include JB/setup %}


<br/>

{% for post in site.posts limit: 4 %}
<div class="row">
	<div class="col-lg-1 vcenter">
		<div class="date">
		{{ post.date | date_to_string | date: "%b %d" }} 
		</div>
	</div>
	<div class="col-lg-11">
		<div class="panel panel-default">
			<div class="panel-heading">
				<a href="{{ BASE_PATH}}{{ post.url }}">{{ post.title }}</a><br/>
			</div>
			<div class="panel-body">
				{{ post.description }}
			</div>
		</div>
	</div>
</div>
{% endfor %}
<br/>

<div class="row">
	<div class="col-lg-12 text-right">
		<button type="button" class="btn btn-default" id="more-articles">More Articles</button>
	</div>
</div>

<br/>

