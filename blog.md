---
layout: blog
permalink: /blog/
lang: ko
---


<ul class="blog-posts">
{% for post in site.posts  %}
	<li>
		<a href="{{ site.url | prepend: site.baseurl }}{{ post.url }}">
			<span class="date">{{ post.date | date: "%d/%m/%Y" }}</span>
			{{ post.title }}

		</a>
        <hr />
	</li>
{% endfor %}
</ul>
