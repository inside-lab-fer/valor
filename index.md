---
alt_url: /en/
---
{%- assign t = site.data.i18n.hr -%}
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

Veliki jezični modeli sve češće sudjeluju u donošenju odluka, a vrijednosti i preferencije koje pritom slijede teško je uočiti i provjeriti. Moćni, ali neusklađeni sustavi umjetne inteligencije predstavljaju ozbiljan praktični rizik, a postojeće metode za razumijevanje i usklađivanje vrijednosti takvih sustava još su ograničene.

Projekt **Vrijednosno usklađeno i interpretabilno optimiranje i rasuđivanje (VALOR)** razvija metode za interpretabilnost i usklađivanje vrijednosti velikih jezičnih modela (LLM-ova) u procesima optimizacije i rasuđivanja. Navedeni cilj možemo podijeliti na:

1. razvoj metoda koje omogućuju bolje razumijevanje načina na koji modeli donose odluke,
2. razvoj tehnika za praćenje i usmjeravanje ponašanja modela prema ciljnim vrijednostima,
3. izradu otvorenih testnih skupova i alata za procjenu usklađenosti vrijednosti.

</section>

<section id="tim">
  <h2>{{ t.team }}</h2>
  {% include team.html %}
</section>

<section id="vijesti">
  <div class="section-head"><h2>{{ t.news }}</h2><a href="{{ t.news_url | relative_url }}">{{ t.all_news }} →</a></div>
  {% include news-list.html lang="hr" limit=6 %}
</section>

<section id="radovi">
  <h2>{{ t.pubs }}</h2>
  {% include pubs.html lang="hr" %}
</section>
</main>
