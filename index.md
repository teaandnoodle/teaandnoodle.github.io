---
layout: default
title: 我的Blog
tags: [jekyll, github, git, markdown]
---

##{{ page.title }}
* 最新文章
{% for post in site.posts %}
	* {{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{% endfor %}