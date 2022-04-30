---
layout: pages
title: Summer 2021
description: Issue 08 of LIGEIA Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/summer2021_og/coverimage.jpg'
width: 800
height: 418
---
{% include issue-jumbotron.html %}
<div class="container mt-4">

<div class="row">
	<div class="col-md px-4 px-md-3">

	<img src="{{ '/assets/img/summer2021/paul-cristina-abstract_portrait.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Mai Vo-Dinh"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Abstract Portrait Study no.2</cite> by <a href="https://www.paulcristina.com/" target="_blank">Paul Cristina</a>.</footer>

	<img src="{{ '/assets/img/summer2021/xiaofu-wang-introvert.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Mai Vo-Dinh"/>
	<footer class="blockquote-footer mb-3"> <cite title="Source Title">Introvert</cite> by <a href="https://www.wang-xiaofu.org/" target="_blank">Xiaofu Wang</a>.</footer>


	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.summer-2021 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/summer2021/dichotomy.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art by Wendell Poindexter" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Dichotomy</cite> by Wendell Poindexter.</footer>

		<img src="{{ '/assets/img/summer2021/childhood-home-yehui-zhao.jpg'  | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Yehui Zhao" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Childhood Home</cite> by <a href="https://www.yehuizhao.com/" target="_blank">Yehui Zhao</a>.</footer>

		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.summer-2021 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/summer2021/reflecting_absence.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Jennifer Shoemaker"/>
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Reflecting Absence</cite> by Jennifer Shoemaker.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.summer-2021 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/summer2021/jackandjill.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Aishwarya Iyer"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Jack and Jill Went Up The Hill and Took LSD</cite> by Vicki Favilla.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.summer-2021 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
