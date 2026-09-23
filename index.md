---
layout: default
title: Головна
---

<section class="hero hero-photo">
  <div>
    <p class="kicker">Євген Кочубей · психолог, гештальт-терапевт · онлайн та у Києві</p>
    <blockquote>«Я ніби живу не своє життя»</blockquote>
    <p class="lede">
      Так часто починається розмова. Зовні все начебто добре — робота, стосунки,
      справи. А всередині — розгубленість, втома чи відчуття, що щось не так,
      і незрозуміло, що саме.
    </p>
    <div class="hero-actions">
      <a class="btn" href="{{ '/kontakty/' | relative_url }}">Записатись на консультацію</a>
      <a class="btn-outline" href="#shlyakhy">Що вам ближче</a>
    </div>
  </div>
  <figure>
    <img src="{{ '/assets/images/portret-holovna.jpg' | relative_url }}"
         alt="Євген Кочубей, психолог і гештальт-терапевт"
         width="900" height="1350" fetchpriority="high">
  </figure>
</section>

<section class="section" id="shlyakhy">
  <h2>З чим до мене приходять</h2>
  <div class="two-paths">
    <div class="path-card">
      <h3>Чоловіки в кризі сенсу</h3>
      <p>
        Функціонуєш нормально — кар'єра, бізнес, сім'я — але всередині втома,
        розгубленість, відчуття, що живеш не своє життя, труднощі з близькістю.
      </p>
      <p><a href="{{ '/choloviky/' | relative_url }}">Детальніше →</a></p>
    </div>
    <div class="path-card">
      <h3>Тривога, стосунки, кризові стани</h3>
      <p>
        Тривога, яка не минає, апатія, складнощі в стосунках, виснаження —
        стани, знайомі багатьом з нас, особливо зараз.
      </p>
      <p><a href="{{ '/zagalni-stany/' | relative_url }}">Детальніше →</a></p>
    </div>
  </div>
</section>

<section class="section-alt">
  <div class="wrap">
    <h2>Самодопомога — безкоштовно</h2>
    <p>
      Бібліотека науково обґрунтованих тестів (тривога, депресія, тип
      прив'язаності та інші), а також практики для самостійної роботи —
      дихальні вправи, техніки заспокоєння, таблиці для роботи з думками.
    </p>
    <p><a href="{{ '/samodopomoga/' | relative_url }}">Перейти до розділу самодопомоги →</a></p>
  </div>
</section>

<section class="section">
  <h2>Останнє в блозі</h2>
  <ul class="post-list">
    {% for post in site.posts limit:4 %}
    <li>
      <div class="post-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
      <div class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 24 }}</div>
    </li>
    {% endfor %}
  </ul>
  <p><a href="{{ '/blog/' | relative_url }}">Усі статті →</a></p>
</section>

<section class="section-alt">
  <div class="wrap">
    <h2>Формат роботи</h2>
    <ul class="list-plain">
      <li>Онлайн (Zoom) або офлайн у Києві</li>
      <li>Індивідуальна консультація — 50 хв, 2000 грн</li>
      <li>Терапевтичні групи — деталі на сторінці груп</li>
      <li>Працюю в гештальт-підході, з елементами КПТ, майндфулнес, екзистенційного аналізу</li>
    </ul>
    <a class="btn" href="{{ '/kontakty/' | relative_url }}">Записатись на консультацію</a>
  </div>
</section>
