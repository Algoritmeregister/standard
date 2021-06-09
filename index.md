---
---
<style>
    table, th, td {
        border: 1px solid black;
        padding: 10px;
    }
</style>
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