---
layout: pages
title: Spring 2023
description: Issue 13 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/spring2023_og/boo-small.jpg'
width: 800
height: 418
---

{% include issue-jumbotron.html %}

<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">
	<img src="{{ '/assets/img/spring2023/angelika.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Leo Park"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Angelika</cite> by <a href="https://leopark.se/" target="_blank">Leo Park</a>.</footer>


	
	<img src="{{ '/assets/img/spring2023/prachi-valechha-goon-color.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Prachi Valechha" />
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Goon Color</cite> by <a href="https://www.instagram.com/rainbowteeth/" target="_blank">Prachi Valechha</a>.</footer>
	</div>

	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.spring-2023 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/spring2023/claire-flath-boo.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Claire Flath"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Boo</cite> by <a href="https://www.claireflath.com/" target="_blank">Claire Flath</a>.</footer>
		<img src="{{ '/assets/img/spring2023/untitled-jean-yoo.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Jean Yoo" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Untitled</cite> by <a href="https://jeanyoo.com/" target="_blank">Jean Yoo</a>.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.spring-2023 | where: "tags", "fiction" %}
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
	<img src="{{ '/assets/img/spring2023/forget-me-not.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Se Jong Cho" />
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Forget Me Not</cite> by <a href="https://sejongee.com/" target="_blank">Se Jong Cho</a>.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.spring-2023 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/spring2023/jg-orudjev-transcendence.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by J G Orudjev"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Transcendence</cite> by <a href="https://www.nineteendegrees.net/" target="_blank">J G Orudjev</a>.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.spring-2023 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
