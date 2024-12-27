---
layout: blog
title: "Blog"
---

<div id='posts' class='section'>
    {% for post in site.posts %}
        <div class='post-row'>
            <p class='post-title'>
                <a href="{{ post.url }}">
                    {{ post.title }}
                </a>
            </p>
            <p class='post-date'>
                {{ post.date | date_to_long_string }}
            </p>
        </div>
        <p class='post-subtitle'>
            {{ post.subtitle }}
        </p>
    {% endfor %}
</div>
