---
layout: default
---

<div>
    <div>
        <div class="caption">Recent Blogs</div>

        <ul>
        {% for post in site.posts %}
            <li>
		{{ post.date | date: '%b. %-d, %Y' }}	
                <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                <div>{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>
    </div>
</div>
