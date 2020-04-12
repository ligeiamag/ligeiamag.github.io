---
layout: pages
title: Spring 2020
description: Issue 03 of Ligeia Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/spring2020_og/phyllis.jpg'
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
	<img src="{{ '/assets/img/spring2020/p-07.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Kailey Barthel" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">No one saw you come in, no one saw you leave</cite> by <a href="https://www.kaileybarthel.com/" target="_blank">Kailey Barthel</a> </footer>
		<img src="{{ '/assets/img/spring2020/p-06.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Photo by Marshall Farren"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Truck Stop/Grocery Store</cite> by Marshall Farren.</footer>
	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.spring-2020 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/spring2020/p-09.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Florence Pinel"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Amazones</cite> by <a href="https://florenceannerosepinel.jimdofree.com/" target="_blank">Florence Pinel</a>.</footer>

		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.spring-2020 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/spring2020/p-08.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Ed Becker" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Inside Voices</cite> by Ed Becker. </footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.spring-2020 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/spring2020/p-05.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art By Phyllis Mayes" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">The Satyr</cite> by <a href="http://www.phyllismayes.com/" target="_blank">Phyllis Mayes</a>.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.spring-2020 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
