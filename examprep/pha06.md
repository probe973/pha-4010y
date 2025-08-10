---
layout: default
title: Exam Prep 6
---
<main>

<h1>Examination Practice Questions 6</h1>

<section class="instructions">
    <h2>Instructions</h2>
    <ul>
                <li>Answer <strong>ALL</strong> questions on this paper.</li>
                <li>All questions have equal weighting.</li>
                <li>All answers must include units, where appropriate. Answers without units (or incorrect units) will be marked as incorrect.</li>
                <li>Calculators of any description are <strong>NOT</strong> allowed.</li>
    </ul>
</section>

<section class="formulae">
    <h2>For Your Information:</h2>
    <p>
        $\sqrt{2.25} = 1.5$, $\sqrt{2.56} = 1.6$, $\sqrt{2.97} = 1.7$, $\sqrt{3.24} = 1.8$, $\sqrt{3.61} = 1.9$, $\sqrt{4.00} = 2.0$,<br>
        $\sqrt{4.41} = 2.1$, $\sqrt{4.84} = 2.2$, $\sqrt{5.29} = 2.3$, $\sqrt{5.76} = 2.4$, $\sqrt{6.25} = 2.5$, $\sqrt{6.76} = 2.6$,<br>
        $\sqrt{7.29} = 2.7$, $\sqrt{7.84} = 2.8$, $\sqrt{8.41} = 2.9$, $\sqrt{9.00} = 3.0$
    </p>
  
</section>

<hr>

<ol>
  {% for p in site.data.pha_06 %}
    {% include problem_builder.html problem=p %}
  {% endfor %}
</ol>

<hr>
</main>
