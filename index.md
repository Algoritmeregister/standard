---
---
<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>
<br>
<table>
    <tr>
        <th>name</th>
        <th>category</th>
        <th>type</th>
        <th>description</th>
        <th>required</th>
    </tr>
    {% for property in site.data.schema-v0_2.properties %}

        <tr>
            <td>{{ property.name }}</td>
            <td>{{ property.category }}</td>
            <td>{{ property.type }}</td>
            <td>{{ property.description }}</td>
            <td>{{ property.required }}</td>
        </tr>

    {% endfor %}
</table>
