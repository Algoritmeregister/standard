---
---
EN: These are the definitions that are being formalized by the consortiumpartners.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">View this project on Github</a>

NL: Dit zijn de definities die zijn vastgesteld tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>

<br>
<table>
    <tr>
        <th>Variable name / naam van de variabele</th>
        <th>Name</th>
        <th>Naam (nl)</th>
        <th>Description</th>
        <th>Omschrijving (nl)</th>
    </tr>
    {% for term in site.data.glossary %}
    <tr>
        <td><pre>{{ term[0] }}</pre></td>
        <td>{{ term[1].name }}</td>
        <td>{{ term[1].translations.nl.name }}</td>
        <td>{{ term[1].description }}</td>
        <td>{{ term[1].translations.nl.description }}</td>
    </tr>
    {% endfor %}
</table>
