---
title: "Posts"
layout: default
---

# Posts

Browse all posts and stories from this collection.

{% for post in site.posts %}
  <div class="post-item">
    <h2>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </h2>
    <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
    <p>{{ post.excerpt }}</p>
  </div>
{% endfor %}

{% if site.posts.size == 0 %}
  <p>No posts yet. Check back soon!</p>
{% endif %}
