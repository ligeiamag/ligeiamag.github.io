---
layout: pages
title: Summer 2020
description: Issue 04 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/summer2020/luanne.jpg'
width: 600
height: 746
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
		<img src="{{ '/assets/img/summer2020/joe.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Photo by Joe Lugara"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">v703</cite> by <a href="https://joelugara.com/" target="_blank">Joe Lugara</a>.</footer>
	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.summer-2020 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/summer2020/luanne.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Luanne Redeye" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">83-J</cite> by <a href="https://luanneredeye.com/" target="_blank">Luanne Redeye</a>. Gouache on Wood. </footer>
			<img src="{{ '/assets/img/summer2020/jim-zola.jpeg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Jim Zola"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Untitled</cite> by Jim Zola.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.summer-2020 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/summer2020/garni.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Photo By Ricky Garni" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Rally For Justice: Chapel Hill, North Carolina</cite> by Ricky Garni.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.summer-2020 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/summer2020/edram.jpeg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art By Ed Ramsburg" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Untitled</cite> by Ed Ramsburg.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.summer-2020 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
