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
    </tr>
    {% for item in site.data.schema-v0_2.properties %}

        <tr>
            <td>{{ item[1].name }}</td>
            <td>{{ item[1].category }}</td>
            <td>{{ item[1].type }}</td>
            <td>{{ item[1].description }}</td>
        </tr>

    {% endfor %}
</table>
