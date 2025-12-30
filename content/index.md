---
layout: base.njk
permalink: /
---

<div class="row">
    <div class="col c12">
        <h1>Welcome to Minimalist Crow</h1>
        <p>{{ metadata.description }}</p>
    </div>
</div>

<div class="row">
    <div class="col c12">
        <h2>Recent Posts</h2>
    </div>
</div>

<div class="row">
    {%- for post in collections.posts | slice(0, 3) %}
    <div class="col c4">
        <h3><a href="{{ post.url }}">{{ post.data.title }}</a></h3>
        <p class="post-meta">{{ post.date | readableDate }}</p>
        <p>{{ post.data.excerpt or post.content | striptags | truncate(150) }}</p>
        <p><a href="{{ post.url }}">Read more →</a></p>
    </div>
    {%- endfor %}
</div>

<div class="row" style="margin-top: 2em;">
    <div class="col c12">
        <p><a href="/blog/" class="btn btn-a">View all posts</a></p>
    </div>
</div>
