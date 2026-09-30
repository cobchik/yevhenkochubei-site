---
layout: default
title: Самодопомога
description: "Безкоштовні анонімні тести на тривожність (GAD-7), депресію (PHQ-9) і тип прив'язаності та практики самодопомоги: дихання, розслаблення тіла, робота з думками."
permalink: /samodopomoga/
---

<section class="hero">
  <h1>Самодопомога</h1>
  <p class="lede">
    Терапія — це лише один зі способів собі допомогти. В цьому розділі викладено науково
    обґрунтовані тести для самодіагностики та практики, якими можна
    користуватись самостійно. Все безкоштовно.
  </p>
  {% include crisis.html short=true %}
</section>

<section class="section">
  <h2>Тести</h2>
  <p class="post-excerpt">
    Усі тести — валідовані наукові інструменти. Це скринінг, а не діагноз:
    після проходження ви отримаєте інтерпретацію та рекомендацію, до кого
    звернутись, якщо результат про це говорить.
  </p>

  {% comment %}
    Список тестів будується автоматично з файлів у папці samodopomoga/.
    Тест з'являється тут, щойно його сторінка опублікована (без published: false).
  {% endcomment %}
  {% assign tests = site.pages | where: "layout", "test" | sort: "title" %}
  <div class="cards cards-3">
    {% for test in tests %}
    <a class="card" href="{{ test.url | relative_url }}">
      <span class="card-label">{{ test.questions }} запитань · {{ test.minutes }} хв</span>
      <span class="card-title">{{ test.title }}</span>
      <span class="card-text">{{ test.summary }}</span>
      <span class="card-more">Пройти тест →</span>
    </a>
    {% endfor %}
  </div>
  <p class="post-excerpt">Нові тести додаються поступово.</p>
</section>

<section class="section-alt">
  <div class="wrap">
    <h2>Практики</h2>
    {% comment %}Список будується автоматично зі сторінок з type: practice{% endcomment %}
    {% assign practices = site.pages | where: "type", "practice" | sort: "title" %}
    <div class="cards cards-3">
      {% for pr in practices %}
      <a class="card" href="{{ pr.url | relative_url }}">
        <span class="card-label">Практика · {{ pr.minutes }} хв</span>
        <span class="card-title">{{ pr.title }}</span>
        <span class="card-text">{{ pr.summary }}</span>
        <span class="card-more">Спробувати →</span>
      </a>
      {% endfor %}
    </div>
    <p class="post-meta">Нові практики додаються поступово.</p>
  </div>
</section>

<section class="section">
  {% include crisis.html %}
</section>
