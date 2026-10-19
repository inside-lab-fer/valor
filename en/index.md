---
alt_url: /
---
{%- assign t = site.data.i18n.en -%}
<section class="hero">
  <div class="wrap">
    <p class="eyebrow">{{ t.eyebrow }} · FER</p>
    <h1>VALOR</h1>
    <p class="subtitle">{{ t.title }}</p>
  </div>
</section>

<main class="wrap">
<section id="projekt" class="about prose" markdown="1">

## {{ t.about }}

Large language models increasingly take part in decision making, while the values and preferences they follow are hard to see and verify. Powerful but misaligned AI systems pose a serious practical risk, and existing methods for understanding and aligning the values of such systems are still limited.

The project **Value-aligned and interpretable optimization and reasoning (VALOR)** develops methods for interpretability and value alignment of large language models (LLMs) in optimization and reasoning processes. This goal breaks down into:

1. methods for better understanding how models make decisions,
2. techniques for monitoring and steering model behaviour towards target values,
3. open benchmark datasets and tools for evaluating value alignment.

</section>

<section id="tim">
  <h2>{{ t.team }}</h2>
  {% include team.html %}
</section>

<section id="vijesti">
  <div class="section-head"><h2>{{ t.news }}</h2><a href="{{ t.news_url | relative_url }}">{{ t.all_news }} →</a></div>
  {% include news-list.html lang="en" limit=6 %}
</section>

<section id="radovi">
  <h2>{{ t.pubs }}</h2>
  {% include pubs.html lang="en" %}
</section>
</main>
