---
layout: page
title: Archive
permalink: /archive/
---

This is the archive of all posts on this site.<br>


  {%- if site.posts.size > 0 -%}
      {%- for post in site.posts -%}
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
	  {%- endif -%}
      {%- endfor -%}
  {%- endif -%}
