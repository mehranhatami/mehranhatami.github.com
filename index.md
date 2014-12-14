---
layout: page
title: JavaScript daily trends ...
tagline: JavaScript
---
{% include JB/setup %}
<ul class="entries">
{% for post in site.posts limit:10 %}
  <li>
    <p>
    	<a href="{{ post.url }}">
	    <h2>{{ post.title }}</h2>
	    </a>
	    <span class="blogdate">{{ post.date | date: "%d %B %Y" }}</span>
	    <div>{{ post.content |truncatehtml | truncatewords: 30 }}</div>
    </p>
  </li>
{% endfor %}
</ul>