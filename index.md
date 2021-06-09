---
---
<a href="https://github.com/tiltshiftnl/algoritmeregister-metadata-standaard">Bekijk de code op Github</a>
<br>
<table>
    <tr>
        <th>naam</th>
        <th>CATEGORIE</th>
        <th>eigenschap</th>
        <th>type</th>
        <th>omschrijving</th>
    </tr>
    {% for item in site.data.algoritmeregister-metadata-standaard %}
    <tr>
        <td>{{ item.naam }}</td>
        <td>{{ item.categorie }}</td>
        <td>{{ item.eigenschap }}</td>
        <td>{{ item.type }}</td>
        <td>{{ item.omschrijving }}</td>
    </tr>
    {% endfor %}
</table>