---
layout: pages
title: Spring 2022
description: Issue 11 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/spring2022_og/esther_ogimage.jpg'
width: 800
height: 418
---

{% include issue-jumbotron.html %}

<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">
	<img src="{{ '/assets/img/spring2022/esther_art.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Esther De Rojas"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Untitled</cite> by <a href="https://www.instagram.com/de_rojas_studio/" target="_blank">Esther De Rojas</a>.</footer>
	<img src="{{ '/assets/img/spring2022/lightner-royal-elm.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Rhee Lightner" />
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Portrait of Royal Elm</cite> by <a href="https://www.rheelightnerstudio.com/" target="_blank">Rhee Lightner</a>.</footer>
	</div>

	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.spring-2022 | where: "tags", "poetry" %}
	{% for item in poems %}
						<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a>
						</p>
						<p class="authortitle"><span class="entryby">By</span> {{item.author}}</p>
	    {% endfor %}
	</div>
</div>
<hr />

<div class="row">
		<div class="col-md px-4 px-md-3">
		<img src="{{ '/assets/img/spring2022/vunerable.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Erik Skytthammar"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Vunerable</cite> by <a href="https://www.instagram.com/erikskytthammar/" target="_blank">Erik Skytthammar</a>.</footer>
		<img src="{{ '/assets/img/spring2022/those-who-come-by-sea.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by By Kim Baglieri"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Those Who Come by Sea</cite> by <a href="https://www.instagram.com/kimthewild/" target="_blank">Kim Baglieri</a>.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.spring-2022 | where: "tags", "fiction" %}
		{% for item in fiction %}
							<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a>
							</p>
							<p class="authortitle"><span class="entryby">By</span> {{item.author}}</p>
		    {% endfor %}
		</div>
	</div>
<hr />

  <div class="row">
    <div class="col-md px-4 px-md-3">
		<img src="{{ '/assets/img/spring2022/marta-wonder.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Diana Marta"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">I Wonder</cite> by Diana Marta.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.spring-2022 | where: "tags", "nonfiction" %}
			{% for item in nonfiction %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a>
								</p>
								<p class="authortitle"><span class="entryby">{% if item.reviewer %} reviewed {% endif %} By</span> {{item.author}}</p>
					{% endfor %}
		</div>
  </div>
  <hr />

	<div class="row">
	  <div class="col-md px-4 px-md-3">
		<img src="{{ '/assets/img/spring2022/concrete-ice-cream.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Mario Loprete" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Concrete Ice Cream</cite> by <a href="https://www.instagram.com/marioloprete/" target="_blank">Mario Loprete</a>.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.spring-2022 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
