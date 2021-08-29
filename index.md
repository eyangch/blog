## eyangch's blog

huh
{% assign posts = site.posts %}
{%- if posts.size > 0 -%}
  {%- if page.list_title -%}
    <h2 class="post-list-heading">{{ page.list_title }}</h2>
  {%- endif -%}
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
  {%- for post in posts -%}
  <h3>
    <a class="post-link" href="{{ post.url | relative_url }}">
      {{ post.title | escape }} [{{ post.date | date: date_format }}]
    </a>
  </h3>
  {%- if site.show_excerpts -%}
    {{ post.excerpt }}
  {%- endif -%}
  {%- endfor -%}
{%- endif -%}
