---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: index
---
## My personal blog
{% for post in site.posts %}
<p>
    <a href="{{ baseurl }}{{ post.url }}">[{{ post.date | date: "%Y/%m/%d" }}] {{ post.title }}</a>
</p>
{% endfor %}
