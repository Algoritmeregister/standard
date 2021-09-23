---
---
<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>
<br>
<table>
    <tr>
        <th>attribute</th>
        <th>name</th>
        <th>category</th>
        <th>type</th>
        <th>description</th>
        <th>required</th>
    </tr>
    {% for property in site.data.schema-v0_2.properties %}
        <tr>
            <td>{{ property.attribute }}</td>
            <td>{{ property.name.en }} /<br>{{ property.name.nl | default "<b>nog geen vertaling</b>" }}</td>
            <td>{{ property.category.en }} /<br>{{ property.category.nl | default "<b>nog geen vertaling</b>"  }}</td>
            <td>{{ property.type }}</td>
            <td>{{ property.description.en }} /<br>{{ property.description.nl | default "<b>nog geen vertaling</b>"  }}</td>
            <td>{{ property.required }}</td>
        </tr>

    {% endfor %}
</table>
