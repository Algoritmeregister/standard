---
permalink: /comparison
title: Comparison UK/NL Standard
description: Comparison between the UK and NL standard for algorithmic transparency
---
<body>
<h1>Mapping</h1>
<style>
    body {
        font-family: arial;
    }
</style>
{% assign mapping = site.data.mapping-NL-UK-properties %}
{% assign NL_props = site.data.schema-v0_2.properties %}
{% assign UK_props = site.data.schema-UK-generated.properties %}

{% for prop in mapping %}
    <div style="padding: 10px">
        {% case prop.status %}
        {% when "same" %} ✔️
        {% when "similar" %} 🔔
        {% when "different" %} ⚠️
        {% when "missing" %} ⛔
        {% endcase %}
        UK:<b>{{ prop.UK }}</b> matches NL:<b>{{ prop.NL }}</b> {% if prop.remark %}<i>(notice: {{ prop.remark}})</i>{% endif %}
    </div>
{% endfor %}

<h2>Not yet added to the mapping</h2>

<div style="display: flex">
<div style="flex: 1">
{% for UK_prop in UK_props %}
    {% assign prop = mapping | where: "UK", UK_prop.attribute | first %}
    {% if prop %}
    {% else %}
    <div style="padding: 10px">
        <b>{{ UK_prop.description.en }}</b>
        <pre>
- UK: {{ UK_prop.attribute }}
  NL: 
  remark:
        </pre>
    </div>
    {% endif %}
{% endfor %}
</div>

<div style="flex: 1">
{% for NL_prop in NL_props %}
    {% assign prop = mapping | where: "NL", NL_prop.attribute | first %}
    {% if prop %}
    {% else %}
    <div style="padding: 10px">
        <b>{{ NL_prop.description.en }}</b>
        <pre>
- NL: {{ NL_prop.attribute }}
  UK: 
  remark:
        </pre>
    </div>
  {% endif %}
{% endfor %}
</div>
</div>

<!--
{% assign NL_prop = NL_props | where: "attribute", UK_prop.attribute | first %} 
{{ UK_prop.attribute }}:
    UK: {{ UK_prop.attribute }} - {{ UK_prop.description.en }}
    NL: {{ NL_prop.attribute }} - {{ NL_prop.description.en }}

{% assign UK_prop = UK_props | where: "attribute", NL_prop.attribute | first %}
    {% if UK_prop.attribute %}
    {% else %}
        {{ NL_prop.attribute }}:
            NL: {{ NL_prop.attribute }} - {{ NL_prop.description.en }}
            UK: {{ UK_prop.attribute }} - {{ UK_prop.description.en }}
    {% endif %}
-->