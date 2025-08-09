---
layout: default
title: Imperial/Metric Questions
---
<main>

<h1>Conversion Practice Sheet</h1>

<section class="instructions">
    <h2>Instructions</h2>
    <ul>
        <li>No calculators. Use the assumptions provided in the questions.</li>
    </ul>
</section>

<hr>

<ol>
    {% for question in site.data.imp_met %}
        {% include question_imp_met.html q=question %}
    {% endfor %}
</ol>

<hr>
</main>
