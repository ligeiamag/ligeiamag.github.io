---
layout: pages
title: Winter 2021
description: Issue 10 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/winter2021_og/cyber.jpg'
width: 800
height: 418
---
{% include issue-jumbotron.html %}
<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">

	<img src="{{ '/assets/img/winter2021/jctartwork.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by By Jai Curtis Tui"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">hajime no ippo</cite> by <a href="https://www.instagram.com/jctpaintings/" target="_blank">Jai Curtis Tui</a>.</footer>
	<img src="{{ '/assets/img/winter2021/controlroom1.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Tina Scarpello"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Control Room</cite> by <a href="https://www.instagram.com/tinascarpello/" target="_blank">Tina Scarpello</a>.</footer>
	</div>

	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.winter-2021 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/winter2021/yaching.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Yaching Cheung"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Cyber Mushroom</cite> by <a href="https://yachingcheung.com/" target="_blank">Yaching Cheung</a>.</footer>
		<img src="{{ '/assets/img/winter2021/chosenone.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Kristin LaFollette" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Chosen One</cite> by <a href="https://www.kristinlafollette.com/" target="_blank">Kristin LaFollette</a>.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.winter-2021 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/winter2021/the-bald-clown.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Phyllis Mayes"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">The Bald Clown</cite> by <a href="http://www.phyllismayes.com/" target="_blank">Phyllis Mayes</a>.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.winter-2021 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/winter2021/thumbalina.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Paul Giamattii" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Thumbalina</cite> by <a href="https://linktr.ee/Paulgiamattii" target="_blank">Paul Giamattii</a>.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.winter-2021 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
