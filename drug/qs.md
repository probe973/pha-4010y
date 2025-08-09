---
layout: default
title: Drug Administration Rates
---
<main>

<h1>Drug Administration Rates</h1>

<section class="instructions">
    <h2>Instructions</h2>
    <ul>
        <li>No calculators.</li>
    </ul>
</section>

<hr>

<ol>
    {% for question in site.data.drug_rates %}
        {% include question_drug_rates.html q=question %}
    {% endfor %}
</ol>

<hr>
</main>
