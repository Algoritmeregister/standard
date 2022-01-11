---
---
<a href="https://github.com/algoritmeregister/algoritmeregister-metadata-standaard">Bekijk de code op Github</a>
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
<h1>Formulier Inzet van Algoritme</h1>
<p>Dit formulier is in ontwikkeling. Opmerkingen zijn erg welkom in de kantlijn.</p>
<br>
<form>
{% assign schema = site.data.schema-v0_2 %}
    {% for property in schema.properties %}
    <div class="eigenschap">
        <h2><span class="label">{{ property.category.nl }}</span><br>
            {{ property.name.nl }} (<code>{{ property.attribute }}</code>)</h2>
        <p>{{ property.description.nl }}</p>
        <div class="{{ property.type }}-invoer"></div>
    </div>
{% endfor %}
</form>