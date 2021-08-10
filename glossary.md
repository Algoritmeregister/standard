---
---
EN: These are the definitions that are being formalized by the consortiumpartners.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">View this project on Github</a>

NL: Dit zijn de definities die zijn vastgesteld tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>

<br>
<table>
    <tr>
        <th>Name / naam</th>
        <th>Description / omschrijving</th>
    </tr>
    {% for term in site.data.glossary %}
    <tr>
        <td>{{ term.name }}</td>
        <td>{{ term.description }}</td>
    </tr>
    {% endfor %}
</table>
