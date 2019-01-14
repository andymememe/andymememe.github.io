<a href="https://github.com/andymememe" class="btn cbtn">Github Home</a>
<a href="https://am3devdiary.wordpress.com/" class="btn cbtn">Andy's Dev Diary</a>
<a href="/projects" class="btn cbtn">Feature Projects</a>
<a href="/about" class="btn cbtn">About Me</a>

* * *

{% for category in site.categories %}
## {{ category[0] }}
    {% for post in category[1] %}
 * [{{ post.title }}]({{ post.url }})
    {{ post.excerpt }}
    {% endfor %}
{% endfor %}