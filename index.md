<table>
    <tr>
    {% for tactic in site.tactics %}
        <td><B><a href="{{ tactic.url }}">{{tactic.title}}</a></b>
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
        </td>
    {% endfor %}
    </tr>
</table>



