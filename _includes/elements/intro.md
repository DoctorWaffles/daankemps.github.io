
{% if page.trailer  %}
{% assign trailerpath = trailerpath | append: "/assets/media/" | append: page.trailer %}
{% include elements/trailer.html url=trailerpath %}
{% endif %}

#### {{page.title}} 
<p class="text-muted">{{page.engine}}, {{ page.date | date: "%Y" }}</p>
> {{page.long_description}}

