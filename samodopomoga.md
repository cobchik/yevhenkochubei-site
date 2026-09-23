---
layout: default
title: Самодопомога
permalink: /samodopomoga/
---

<section class="hero">
  <p class="kicker">Безкоштовно</p>
  <h1>Самодопомога</h1>
  <p class="lede">
    Терапія — лише один зі способів собі допомогти. Тут — науково
    обґрунтовані тести для самодіагностики та практики, якими можна
    користуватись самостійно. Все безкоштовно.
  </p>
</section>

<section class="section">
  <h2>Тести</h2>
  <p class="post-excerpt">
    Усі тести — валідовані наукові інструменти. Це скринінг, а не діагноз:
    після проходження ви отримаєте інтерпретацію та рекомендацію — до кого
    звернутись, якщо результат про це говорить.
  </p>

  {% comment %}
    Список тестів будується автоматично з файлів у папці samodopomoga/.
    Тест з'являється тут, щойно його сторінка опублікована (без published: false).
  {% endcomment %}
  {% assign tests = site.pages | where: "layout", "test" | sort: "title" %}
  <ul class="list-plain">
    {% for test in tests %}
    <li><a href="{{ test.url | relative_url }}">{{ test.title }}</a></li>
    {% endfor %}
  </ul>
  <p class="post-excerpt">Нові тести додаються поступово.</p>
</section>

<section class="section-alt">
  <div class="wrap">
    <h2>Практики</h2>
    <p>Готуються до публікації:</p>
    <ul class="list-plain">
      <li>Дихальні вправи для заспокоєння</li>
      <li>Техніки "заземлення" при тривозі</li>
      <li>Короткі медитації</li>
      <li>Таблиця для роботи з тривожними думками (КПТ)</li>
    </ul>
  </div>
</section>
