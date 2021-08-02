---
---
Dit zijn de definities die zijn vastgesteld tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>

<br>
<table>
    <tr>
        <th>Begrip</th>
        <th>Omschrijving</th>
    </tr>
    {% for begrip in site.data.definitions %}
    <tr>
        <td>{{ begrip.naam }}</td>
        <td>{{ begrip.omschrijving }}</td>
    </tr>
    {% endfor %}
</table>
