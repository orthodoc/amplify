---
  layout: page
  title:
  permalink: /articles/
---
{% if site.articles[0] %}
### Articles

<ul class="article-list">
  {% for article in site.articles %}
    <li>
      <a href="{{ site.baseurl }}{{ article.url }}index.html">
        {{ article.title }}
      </a> <span>•</span>
      {% include read_time.html %}
    </li>
  {% endfor %}
</ul>
{% else %}
### Drafts
  {% for article in site.articles %}
    {% unless article.published %}
      {% capture count %}{{ count | plus: 1 }}{% endcapture %}
    {% endunless %}
  {% endfor %}
  {{ count }} articles are being dusted and prepared for the site. Come back later to check them out here.
{% endif %}
