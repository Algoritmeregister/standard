---
---
Dit zijn de user stories die zijn opgehaald tijdens de verschillende inventarisatiesessies met consortiumpartners en genodigden.

<a href="https://github.com/tiltshiftnl/algoritmeregister-metadata-standaard">Bekijk de code op Github</a>

<br>
<table>
    <tr>
        <th>ID</th>
        <th>Story</th>
        <th>Doelgroep</th>
        <th>Bruikbaar</th>
        <th>Opmerkingen</th>
    </tr>
    {% for item in site.data.user-stories %}
    <tr>
        <td>{{ item.ID }}</td>
        <td>{{ item.Story }}</td>
        <td>{{ item.Doelgroep }}</td>
        <td>{{ item.Bruikbaar }}</td>
        <td>{{ item.Opmerkingen }}</td>
    </tr>
    {% endfor %}
</table>
