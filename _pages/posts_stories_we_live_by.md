---
layout: default
permalink: /posts/stories-we-live-by/
title:
---

<cat-nav>
  <a href="{{ site.baseurl }}/posts/all">All</a>
  <a href="{{ site.baseurl }}/posts/story-fundamentals">Story Fundamentals</a>
  <a href="{{ site.baseurl }}/posts/story-analysis">Story Analysis</a>
  <a style="color:#729FCF" href="{{ site.baseurl }}/posts/stories-we-live-by">Stories We Live By</a>
</cat-nav>

<hr>

<div class="posts">
  {% for post in site.categories['Stories We Live By'] %}
    <article class="post">
      <h1>
          <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h1>
      <div>
        <p class="post_date">{{ post.date | date: "%B %e, %Y" }}</p>
      </div>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">
          Read More
      </a>
    </article>
  {% endfor %}
</div>