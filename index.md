---
layout: page
title: lookininward
tagline: a place for my thoughts
---
{% include JB/setup %}


<br/>

<!-- <div class="jumbotron">
  <div class="container">
    <img src="assets/images/forest-light.jpg" class="img-responsive">
  </div>
</div> -->


<div class="row">
	<div class="col-lg-10">
	{% for post in site.posts limit: 4 %}
		<div class="panel panel-default">
			<div class="date">
			{{ post.date | date_to_string | date: "%b %d" }} 
			</div>
			<div class="panel-heading">
				<a href="{{ BASE_PATH}}{{ post.url }}">{{ post.title }}</a><br/>
			</div>
			<div class="panel-body">
				{{ post.description }}
			</div>
		</div>
		{% endfor %}
	</div>
<!-- 	  <div class="col-lg-2">
          <a href="#" class="thumbnail">
            <img src="/assets/images/clients/ehealth-logo.jpg" class="responsive">
          </a>
        </div> -->
</div>

<br/>


      

<div class="row">
	<div class="col-lg-10 text-right">
		<a href="/archive"><button type="button" class="btn btn-default" id="more-articles">More Articles</button></a>
	</div>
</div>

<br/>

