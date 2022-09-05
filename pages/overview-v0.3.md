---
layout: null
permalink: overview
---
<html>
<head>
<style>
    h2 { color: darkblue }
    body { font-family: arial; line-height: 1.4em }
    code { background: darkblue; color: white; padding: 2px }
    .required { background: darkred }
    nav { background: darkblue; position: fixed; padding: 1em }
    nav a { color: white }
    main { max-width: 32em; position: absolute; left: 14em }
    .light {font-size: 0.9em; color: gray }
    @media print {
        main {position: relative; left: 0; margin: auto;}
        nav {display: none;}
        .pb {page-break-before: always;}
    }
</style>
</head>
<body>
<nav>
{% assign tmp = 0 %}
{% assign schema = site.data.schema-v0_3 %}
{% for property in schema.properties %}
{% if tmp != property.category.en %}
    <p><a href="#{{ property.category.en }}">{{ property.category.en }}</a></p>
{% endif %}
{% assign tmp = property.category. en %}
{% endfor %}
</nav>

<main>
{% assign tmp = 0 %}
{% assign schema = site.data.schema-v0_3 %}
{% for property in schema.properties %}
    {% if tmp != property.category.en %}
    <a name="{{ property.category.en }}"></a>
    <h2 {% if tmp != 0 %}class="pb"{% endif %}>{{ property.category.en }}</h2>
    {% endif %}
    {% assign tmp = property.category.en %}
    <p>
        <b>► {{ property.name.en }}</b>
        <code {% if property.required %}class="required"{% endif %}>{{ property.attribute }}</code>
        {% if property.required %} <span class="light">(required)</span>{% endif %}<br>
        <i>{{ property.description.en }}{% if property.examples.en %}<br>
            <span class="light">Examples: {{ property.examples.en }}</span>{% endif %}</i>
    </p>
    <p>type: <b>{{ property.type }}</b></p>
    {% if property.enum.en %}
        Possible values:<br><br>
        {% for value in property.enum.en %}
            <code style="margin-left: 2.4em">{{ value }}</code><br>
        {% endfor %}
    {% endif %}
{% endfor %}

</main>
</body>
</html>