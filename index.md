# Andy's Projects

{% for repository in site.github.public_repositories %}
    {% unless repository.name contains '.' %}
* [{{ repository.name }}]({{ repository.html_url }})
    {% endunless %}
{% endfor %}
