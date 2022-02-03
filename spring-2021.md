---
layout: pages
title: Spring 2021
description: Issue 07 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/spring2021_og/ideation.jpg'
width: 800
height: 418
---
<div class="jumbotron jumbotron-fluid padding-main">
	<div class="container h-100">
		<div class="row h-100">
			<div class="col text-center my-auto pb-4">
				<div class="m-3 p-2 m-md-4 p-md-3">
					<h1 class="text-center display-4  ligeia-title">
            Ligeia
          </h1>
				</div>
			</div>
		</div>
	</div>
</div>
<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">

	<img src="{{ '/assets/img/spring2021/P1340796.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Mai Vo-Dinh"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Untitled</cite> by Mai Vo-Dinh.</footer>

	<img src="{{ '/assets/img/spring2021/aishwarya-iyer.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Aishwarya Iyer"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">weather</cite> by <a href="https://www.instagram.com/aisiyer/" target="_blank">Aishwarya Iyer</a>.</footer>
	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.spring-2021 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/spring2021/watchful.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Jennifer Shoemaker" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">The Watchful Eye (The Shaman)</cite> by <a href="https://www.bedotgallery.com/jen-butt-be-dot-gallery" target="_blank">Jennifer Shoemaker</a>.</footer>
			<img src="{{ '/assets/img/spring2021/Marta_Ideation_1.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art By Diana Marta" />
				<footer class="blockquote-footer mb-3"> <cite title="Source Title">Ideation</cite> by Diana Marta.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.spring-2021 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/spring2021/bigmouth.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Marilyn Whitehorse" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Big Mouth</cite> by Marilyn Whitehorse.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.spring-2021 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/spring2021/garden.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Ed Ramsburg"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Garden of Earthly Delights</cite> by Ed Ramsburg.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.spring-2021 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
