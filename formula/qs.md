---
layout: default
title: Formula Scaling
---
<main>

<h1>Formula Scaling</h1>

<section class="instructions">
    <h2>Instructions</h2>
    <ul>
        <li>No calculators.</li>
    </ul>
</section>

<hr>

<ol>
    {% for question in site.form_scaling %}
        {% include question_form_scale.html q=question %}
    {% endfor %}
</ol>

<hr>
</main>
