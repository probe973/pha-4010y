---
layout: default
title: Debug Test
---

<main>
<h1>Debug Test Page</h1>
<hr>

<h2>Testing the first data entry directly:</h2>

{% assign first_item = site.data.drug_rates[0] %}

<p>Found data: {{ first_item | inspect }}</p>

{% assign time_in_hours = first_item.time %}
{% assign rate_mcg_min = first_item.rate %}

<p>Time (hours): {{ time_in_hours }}</p>
<p>Rate (mcg/min): {{ rate_mcg_min }}</p>

{% assign time_in_minutes = time_in_hours | times: 60 %}
{% assign total_mcg = time_in_minutes | times: rate_mcg_min %}
{% assign total_mg = total_mcg | divided_by: 1000.0 %}

<p>Time in Minutes (calculated): {{ time_in_minutes }}</p>
<p>Total MCG (calculated): {{ total_mcg }}</p>
<p>Total MG (calculated): {{ total_mg }}</p>

<hr>
<h2>The final output should be here:</h2>

<ol>
<li>If a paitent requires <strong>{{ rate_mcg_min }} mcg/min </strong> for <strong>{{time_in_hours}} hours</strong>, what is the total amount of drug they will require in <strong>milligrams</strong>?
    <details>
        <summary>Solution</summary>
        <div>
          <p>Step 1: Convert the hours into minutes: </p>
          <p>${{time_in_hours}} \times 60 = {{ time_in_minutes }}$</p>
          <p>Step 2: Find total micrograms: </p>
          <p>${{rate_mcg_min}} \text{mcg/min} \times {{ time_in_minutes }} \text{min} = {{ total_mcg }} \text{mcg} $</p>
          <p>Step 3: Convert to milligrams: </p>
          <p> ${{total_mcg}} \div 1000 = {{total_mg}} $</p>
          <p><strong>Solution: {{total_mg}} mg</strong></p>
        </div>
    </details>
</li>
</ol>

</main>
