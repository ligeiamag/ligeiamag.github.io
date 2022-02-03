---
layout: pages
title: Winter 2020
description: Issue 06 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/winter2020_og/greg.jpg'
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
	<img src="{{ '/assets/img/winter2020/imreading.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Megan McNitt"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">I'm Reading</cite> by <a href="https://www.instagram.com/mcnitt_megan/" target="_blank">Megan McNitt</a>.</footer>
	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.winter-2020 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/winter2020/space.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art By Courtney Applequist" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">The Space Between</cite> by <a href="https://courtneyapplequist.com/" target="_blank">Courtney Applequist</a> | <a href="https://www.instagram.com/courtneyapplequistart/" target="_blank">@courtneyapplequistart</a></footer>
		<img src="{{ '/assets/img/winter2020/dArtBecker.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Ed Becker" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">D</cite> by Ed Becker.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.winter-2020 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/winter2020/winter.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Greg McLemore" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">The Blizzard of 2016</cite> by <a href="https://www.gregmclemoreart.com/" target="_blank">Greg McLemore</a>.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.winter-2020 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/winter2020/altar.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Brian Truesdale"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Rebuilding My Altar to Hope</cite> by Brian Truesdale.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.winter-2020 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
