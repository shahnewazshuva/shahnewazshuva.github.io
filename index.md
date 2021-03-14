---
layout: default
---

<!--Text can be **bold**, _italic_, or ~~strikethrough~~.-->

<!-- [**Home**](./index.html)|[**Categories**](./pages/categories.html)|[**Archives**](./pages/archives.html) -->

<!--
<ul id="posts">

	{% for post in paginator.posts %}

	  <li class="post">
	  	<h2><a href="{% if site.baseurl == "/" %}{{ post.url }}{% else %}{{ post.url | prepend: site.baseurl }}{% endif %}">{{ post.title }}</a></h2>
	  	<time datetime="{{ post.date | date_to_xmlschema }}" class="by-line">{{ post.date | date_to_string }}</time>
	  	<p>{{ post.content | strip_html | truncatewords:50 }}</p>
	  </li>

    {% endfor %}

</ul>  -->

<h2>Latest Posts</h2>
<ul>
  {% for post in site.posts %}
    <li style="list-style-type:none;" >
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p><small> Posted on <time datetime="{{ post.date | date_to_xmlschema }}" class="by-line">{{ post.date | date_to_string }}</time> by <a href="/pages/aboutme.html">{{post.author}}</a> </small></p>
      <p>{{ post.content | strip_html | truncatewords:50 }}</p>

    </li>
  {% endfor %}
</ul>
