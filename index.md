# Andy's Projects

{% for repository in site.github.public_repositories %}
    {% assign counter = 5 %}
    {% unless repository.name contains '.' or counter <= 0 %} 
  * [{{ repository.name }}]({{ repository.html_url }})
        {% decrement counter %}
    {% endunless %}
{% endfor %}
* [More](/projects)
