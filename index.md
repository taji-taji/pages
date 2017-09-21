# Today I Learned

## Latest

<ul>

{% for post in site.posts %}

<li>
  <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}<small>[{{ post.date }}]</small></a>
</li>

{% endfor %}

</ul>


## Categories

{% assign category_names = "" | split: "|"  %}

{% for posts_by_category in site.categories %}
  {% assign category_names = category_names | push: posts_by_category.first %}
{% endfor %}

{% assign category_names = category_names | sort %}

<ul>

{% for category_name in category_names %}
<li>
  {{ category_name }}
</li>
{% endfor %}

</ul>
