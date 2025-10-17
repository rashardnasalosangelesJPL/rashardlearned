---
layout: post
mermaid: true
published: true
title: "Listing Posts in LiQUiD "
tags: computing jekyll programming webdesign blogging tips
catagories: computing jekyll programming webdesign blogging tips
image: post_computingq.PNG

---



# Listing Posts
@jekyll @nasa-jpl @blackgirlscode test bed 



{% for LA in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a></li>
      <article class="paginator">
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
</article>
    {% endfor %}
  </ul>
{% endfor %}

{% raw %}

{% for LA in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a></li>
      <article class="paginator">
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
</article>
    {% endfor %}
  </ul>
{% endfor %}

{% endraw %}


<ul>
    {% for post in site.posts %}
      <li>
          <h2><a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">{{ post.title }}</a></h2>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
          <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
    {% endfor %}
</ul>

{% raw %}

<ul>
    {% for post in site.posts %}
      <li>
          <h2><a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">{{ post.title }}</a></h2>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
          <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
    {% endfor %}
</ul>

{% endraw %}


{% for mars in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

{% raw %}

{% for mars in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

{% endraw %}



  {% for post in site.posts %}
    
<article class="paginator">
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
</article>

  {% endfor %}

{% raw %}

  {% for post in site.posts %}
    
<article class="paginator">
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-post" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
</article>

  {% endfor %}

{% endraw %}



[markdouwn](https://humanwhocodes.com/blog/2019/04/jekyll-hooks-output-markdown/) 
