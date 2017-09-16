# Today I Learned

## Latest

{% for post in site.posts %}

<h3>
  <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
  <br>
  <small>[{{ post.date }}]</small>
</h3>

{% endfor %}


## Categories

{% for category in site.categories %}
<h3>
  {{ category }}
</h3>
{% endfor %}
