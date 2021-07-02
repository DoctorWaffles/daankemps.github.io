
{% if page.trailer_file  %}
{% assign trailerpath = trailerpath | append: "/assets/media/" | append: page.trailer_file %}
{% include elements/trailer.html url=trailerpath %}
{% endif %}

##### {{page.title}} - ({{page.engine}} {{ page.date | date: "%Y" }})
> {{page.long_description}}

