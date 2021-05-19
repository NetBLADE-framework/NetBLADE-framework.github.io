{% for tactic in site.tactics %}
<a href="{{ tactic.url }}">{{tactic.title}}</a>
<ul>
{%for technique in site.techniques %}
    {%if technique.parent == tactic.id %}
    <li><a href="{{ technique.url }}">{{technique.title}}</a></li>
        <ul>
        {%for subtechnique in site.subtechniques %}
            {%if subtechnique.parent == technique.id %}
            <li><a href="{{ subtechnique.url }}">{{subtechnique.title}}</a></li>
            {% endif %}
        {% endfor %}
        </ul>
    {% endif %}
{% endfor %}
</ul>
{% endfor %}



