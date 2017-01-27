---
layout: post
title: 55555
description: 这是一个含diary的目录
image: assets/images/pic05.jpg
category : diary
date : 2018-01-02
---


{% capture categories %}{% for category in site.categories %}{{ category | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign category = categories | split:',' | sort %}
<h5 class="category">分类</h5>
<ul>
    {% for item in (0..site.categories.size) %}{% unless forloop.last %}
    {% capture word %}{{ category[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ word }}">{{ word }}&nbsp;<sup>{{ site.categories[word].size }}</sup></a></li>
    {% endunless %}{% endfor %}
  </ul>


<section id="one" class="tiles">
{% for post in site.posts limit:site.tiles-count %}
<article>
                <span class="image">
                        <img src="{{ post.image }}" alt="" />
                </span>
                <header class="major">
                        <h3><a href="{{ post.url  | relative_url }}" class="link">{{ post.title }}</a></h3>
                        <p>{{ post.description }}</p>
                </header>
        </article>
{% endfor %}
</section>