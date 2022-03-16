---
permalink: form
title: "Print Form: Use of Algorithm (EN)"
description: Form for inventarisation. Under development. Please add suggestions in the margin.
---
<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">View code on Github</a>
<style>
body {
    max-width: 32em;
    margin: auto;
}
form {
    max-width: 32em;
}
.label {
    display: inline-block;
    background: #AAA;
    color: #FFF;
    border-radius: 2px;
    padding: 2px;
    font-size: 0.4em;
    vertical-align: middle;
}
.string-invoer {
    border: 1px solid #000;
    height: 10em;
}
.date-invoer {
    border: 1px solid #000;
    height: 2em;
    width: 10em;
}
.url-invoer {
    border: 1px solid #000;
    height: 2em;
}
.boolean-invoer {
    border: 1px solid #000;
    height: 2em;
    width: 2em;
}
</style>
<br>
<h1>{{ page.title }}</h1>
<p>{{ page.description }}</p>
<br>
<form>
{% assign schema = site.data.schema-v0_2 %}
    {% for property in schema.properties %}
    <div class="eigenschap">
        <h2><span class="label">{{ property.category.en }}</span><br>
            {{ property.name.en }} (<code>{{ property.attribute }}</code>)</h2>
        <p>{{ property.description.en }}</p>
        <div class="{{ property.type }}-invoer"></div>
    </div>
{% endfor %}
</form>