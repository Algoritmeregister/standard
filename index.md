---
title: Index
description: infinite recursion to this page
---
# {{ site.title }}
## {{ site.description }}

{% for page in site.pages %}
<a href="{{ page.url }}">{{ page.title }}</a> - {{ page.description }} (filename: {{ page.name }})
{% endfor %}

<hr>

<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk dit project op Github</a>
<br>
<table>
    <tr>
        <th>attribute</th>
        <th>name</th>
        <th>category</th>
        <th>type</th>
        <th>description</th>
        <th>required</th>
    </tr>
    {% for property in site.data.schema-v0_2.properties %}
        <tr>
            <td><b>{{ property.attribute }}</b></td>
            <td><b>{{ property.name.en }}</b><br>
                   {{ property.name.nl }}</td>
            <td><b>{{ property.category.en }}</b><br>
                   {{ property.category.nl }}</td>
            <td><b>{{ property.type }}</b></td>
            <td><b>{{ property.description.en }}</b><br>
                   {{ property.description.nl }}</td>
            <td><b>{{ property.required }}</b></td>
        </tr>

    {% endfor %}
</table>
