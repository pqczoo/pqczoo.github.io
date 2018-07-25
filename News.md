---
layout: page
title: News
permalink: /news/
order_number: 3
---

Updates from any of the tables will appear as a new post, hopefully linked to a Twitter page too.

<ul>
  {% for post in site.posts %}
    <li>
	<span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
