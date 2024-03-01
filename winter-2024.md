---
layout: pages
title: Winter 2024
description: Issue 14 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/winter2024_og/witch-og.jpg'
width: 800
height: 418
---

{% include issue-jumbotron.html %}

<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">
	<img src="{{ '/assets/img/winter2024/dance-in-pink.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by JC Alfier"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Her dance will awaken in pink</cite> by JC Alfier.</footer>
	</div>

	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.winter-2024 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/winter2024/witch-marybeth-chew.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Marybeth Chew"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Witch</cite> by <a href="https://marybethchew.com/" target="_blank">Marybeth Chew</a>.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.winter-2024 | where: "tags", "fiction" %}
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
	<img src="{{ '/assets/img/winter2024/AFerlito_DanedlionWine.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Ash Ferlito" />
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Dandelion Wine</cite> by <a href="https://www.instagram.com/ashferlito/" target="_blank">Ash Ferlito</a>.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.winter-2024 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/winter2024/shes-sleeping.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Claire Flath"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">She's Sleeping</cite> by Claire Flath.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.winter-2024 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
