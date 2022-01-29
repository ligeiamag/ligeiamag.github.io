---
layout: pages
title: Fiction
description: A list of all fiction published in LIGEIA.
image:
width:
height:
---


{% include pagesintro.html %}

<div class="container">

<div class="row">
{% for issue in site.data.filter_issue.issue_order %}
{% assign test = site[issue]| where: "tags", "fiction" %}
    {% assign fiction = test %}
            {% for item in fiction %}
        <div class="col-sm-6 col-lg-4 py-2">
            <div class="card h-100">
                  <a href="{{ item.url | prepend: site.baseurl  }}" target="_blank"><img class="card-img-top img-fluid" 
                  src="{{ item.image | prepend: site.baseurl }}" alt="Card image cap"></a>
                <div class="card-body">
                    <p class="card-subtitle mb-2 text-muted"><a href="{{ item.issue | prepend: "/" | prepend: site.baseurl }}" target="_blank">{{ item.issue | replace: '-', ' ' | capitalize }}</a></p>
                    <p class="card-title mb-0"><a href="{{ item.url | prepend: site.baseurl }}" target="_blank"><strong>{{ item.title }}</strong></a></p>
                    <p class="card-text pb-3">by {{ item.author }}</p>
                    <p class="card-text pb-3">{{ item.excerpt }}</p>
                </div>
            </div>
        </div>
            {% endfor %}


                {% endfor %}
    </div>


</div>

