---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

# Welcome to Global It Site.

Here's a sample "posts list".

<div class="row">
  {% for post in site.posts %}
    <div class="col-lg-4">
      <h2>{{ post.title }}</h2>
      <p class="text-danger">As of v8.0, Safari exhibits a bug in which resizing your browser horizontally causes rendering errors in the justified nav that are cleared upon refreshing.</p>
      <p>Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. </p>
      <p><a class="btn btn-primary" href="{{ BASE_PATH }}{{ post.url }}" role="button">Read More »</a></p>
    </div>
  {% endfor %}
</div>

<div class="row">
  <ul class="posts">
    {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
</div>



