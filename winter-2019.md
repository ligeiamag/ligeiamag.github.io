---
layout: pages
title: Winter 2019
description: Issue 02 of Ligeia Magazine. Read a great selection of poetry, fiction, nonfiction, and interviews.
image: '/assets/img/winter2019_og/wounded.jpg'
width: 800
height: 418
---
<div class="jumbotron jumbotron-fluid padding-main">
	<div class="container h-100">
		<div class="row h-100">
			<div class="col text-center my-auto pb-4">
				<div class="m-2 p-2 m-md-3 p-md-3">
					<h5 class="text-center issuename pb-5">
            <a href="{{ '/winter-2019' | prepend: site.baseurl }}">Winter 2019</a>
          </h5>
					<h1 class="text-center display-4 font-weight-bold mainpagename">
            Ligeia
          </h1>
				</div>
			</div>
		</div>
	</div>
</div>
<div class="container mt-5">

<div class="row">
	<div class="col-md px-4 px-md-3">
	<img src="{{ '/assets/img/winter2019/baltimore.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Logan Hicks" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Baltimore Dusk – blue</cite> by <a href="http://workhorsevisuals.com" target="_blank">Logan Hicks.</a> Aerosol on Panel.</footer>
		<img src="{{ '/assets/img/winter2019/night_garden.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Painting By Nora Sturges" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">In the Night Garden</cite> by <a href="http://norasturges.com/" target="_blank">Nora Sturges</a>.  Oil on panel.</footer>
	</div>
	<div class="col-md px-4 px-md-3">
	<p class="mb-3 entrytype text-danger h3">Poetry</p>
	{% assign poems = site.winter-2019 | where: "tags", "poetry" %}
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
		<img src="{{ '/assets/img/winter2019/johan_lowie.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Art by Johan Lowie"/>
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Wounded</cite> by Johan Lowie.</footer>
		</div>
		<div class="col-md px-4 px-md-3">
		<p class="mb-3 entrytype text-danger h3">Fiction</p>
		{% assign fiction = site.winter-2019 | where: "tags", "fiction" %}
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
		<img src="{{ '/assets/img/winter2019/fields.jpg' | prepend: site.baseurl }}"   class="img-fluid  rounded" alt="Art By Logan Hicks" />
			<footer class="blockquote-footer mb-3"> <cite title="Source Title">Franconia Field</cite> by <a href="http://www.elizabethashe.com/" target="_blank">Elizabeth Ashe.</a> Acrylic on canvas.</footer>
    </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Nonfiction</p>
			{% assign nonfiction = site.winter-2019 | where: "tags", "nonfiction" %}
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
		<img src="{{ '/assets/img/winter2019/urban_jungle.jpg' | prepend: site.baseurl }}" class="img-fluid rounded" alt="Drawing By Fabio Sassi" />
		<footer class="blockquote-footer mb-3"> <cite title="Source Title">Urban Jungle</cite> by Fabio Sassi.</footer>
	  </div>
		<div class="col-md px-4 px-md-3">
			<p class="mb-3  entrytype text-danger h3">Interviews</p>
			{% assign interviews = site.winter-2019 | where: "tags", "interview" %}
			{% for item in interviews %}
								<p class="entrytitle"><a href="{{ item.url | prepend: site.baseurl }}">{{ item.title | remove: 'Interview'  }}</a>
								</p>
								<p class="authortitle">{{item.interview}}</p>
					{% endfor %}
		</div>
	</div>
</div>
