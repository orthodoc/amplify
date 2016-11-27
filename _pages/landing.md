---
layout: page
title:
permalink: /landing/
redirect_from:
  - /
---

[<amp-img width="600" height="300" layout="responsive" src="/assets/images/landing_headlines.png"></amp-img>]({{"/courses/get-your-free-guide-on-less-is-more" | relative_url }})

You took the mandatory med courses. You spent quality time diligently following what your teachers taught you. You are not deficient in skills. You were different from your techy friends. You wanted to make an impact in the lives of people.

I am here to say --- *you still can*. But first you have to get rid of that feeling of helplessness. You were born to be a leader. Your patients are looking for you to lead them out of their problems. You *cannot do* that by brushing aside your own problems. Learn to be your true self.

The world has transformed while you were busy pouring yourself over medical books and journals. Its not the industry that drives the world any more. The key word is *information*. [The Third Wave](https://goo.gl/88Kj11) is here. The old medical bag has not only gone out of fashion, but has turned irrelevant. Now we need a different set of tools for the digital world. Come with me on a journey to explore the digital landscape! I have a spanking new toolkit for *you*.

You don't have to tread the lonely path anymore! Welcome.

{% if site.articles %}
  {% for article in site.articles limit: 7 %}
    <article class="post" itemscope itemtype="http://schema.org/Article" role="article">
      <div class="article-item">
        <header class="post-header">
          <h4 class="post-title" itemprop="name"><a href="{{ site.baseurl }}{{ article.url }}" itemprop="url">{{ article.title }}</a></h4>
        </header>
        <!--section class="post-excerpt" itemprop="description">
          <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
        </section-->
        <div class="post-meta">
          <time datetime="{{ article.date | date_to_long_string }}">{{ article.date | date_to_long_string }}</time>
        </div>
      </div>
    </article>
  {% endfor %}
{% else %}
  <script async id="_ck_130134" src="https://forms.convertkit.com/130134?v=6"></script>
{% endif %}
