---
permalink: user-stories
title: Algoritmeregister User Stories
description: Dit zijn de user stories die zijn opgehaald tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.
---
# {{ page.title }}

{{ page.description }}

(<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>)

<br>
<table>
    <tr>
        <th>ID</th>
        <th>Story</th>
        <th>Doelgroep</th>
        <th>Bruikbaar</th>
        <th>Opmerkingen</th>
        <th>Prototype</th>
    </tr>
    {% for item in site.data.user-stories %}
    <tr>
        <td>{{ item.ID }}</td>
        <td>{{ item.Story }}</td>
        <td>{{ item.Doelgroep }}</td>
        <td>{{ item.Bruikbaar }}</td>
        <td>{{ item.Opmerkingen }}</td>
        <td>{{ item.Prototype }}</td>
    </tr>
    {% endfor %}
</table>
