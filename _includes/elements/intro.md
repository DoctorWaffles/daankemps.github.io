
{% if page.trailer  %}
{% assign trailerpath = trailerpath | append: "/assets/media/" | append: page.trailer %}
{% include elements/trailer.html url=trailerpath %}
{% endif %}

##### {{page.title}} - ({{page.engine}}, {{ page.date | date: "%Y" }})
> {{page.long_description}}

