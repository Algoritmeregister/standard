---
permalink: /glossary
title: Glossary
description: These are the definitions that are being formalized by the consortiumpartners.
---
# {{ page.title }}

{{ page.description }}

<a href="#nl">Nederlandse vertaling</a>

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">View this project on Github</a>

<br>
<table>
    <tr>
        <th>Variable</th>
        <th>Name</th>
        <th>Description</th>
    </tr>
    {% for term in site.data.glossary %}
    <tr>
        <td><pre>{{ term[0] }}</pre></td>
        <td>{{ term[1].name }}</td>
        <td>{{ term[1].description }}</td>
    </tr>
    {% endfor %}
</table>

<a name="nl"></a>
<h2>Nederlandse vertaling</h2>

Dit zijn de definities die zijn vastgesteld tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>

<br>
<table>
    <tr>
        <th>Variabele</th>
        <th>Naam</th>
        <th>Omschrijving</th>
    </tr>
    {% for term in site.data.glossary %}
    <tr>
        <td><pre>{{ term[0] }}</pre></td>
        <td>{{ term[1].translations.nl.name }}</td>
        <td>{{ term[1].translations.nl.description }}</td>
    </tr>
    {% endfor %}
</table>
