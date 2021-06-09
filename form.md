---
---
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
.tekst-invoer {
    border: 1px solid #000;
    height: 10em;
}
.datum-invoer {
    border: 1px solid #000;
    height: 2em;
    width: 10em;
}
.url-invoer {
    border: 1px solid #000;
    height: 2em;
}
</style>
<br>
<h1>Formulier Inzet van Algoritme</h1>
<p>Dit formulier is in ontwikkeling. Opmerkingen zijn erg welkom in de kantlijn.</p>
<br>
<form>
{% for item in site.data.algoritmeregister-metadata-standaard %}
    <div class="eigenschap">
        <h2>{{ item.naam }} (<code>{{ item.eigenschap }}</code>) <span class="label">{{ item.categorie }}</span></h2>
        <p>{{ item.omschrijving }}</p>
        <div class="{{ item.type }}-invoer"></div>
    </div>
{% endfor %}
</form>