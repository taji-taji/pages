# Today I Learned

{% for post in site.posts %}

<h3>
  <a href="{{ post.baseurl }}{{ post.url }}">{{ post.title }}</a>
  <br>
  <small>[{{ post.date }}]</small>
</h3>

{% endfor %}
