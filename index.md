---
layout: default
title: Психолог і психотерапевт онлайн та в Києві
---

<section class="hero hero-photo">
  <div>
    <h1 class="kicker">Євген Кочубей · клінічний психолог, гештальт-психотерапевт · онлайн та в Києві</h1>
    <blockquote>«Я ніби живу не своє життя»</blockquote>
    <p class="lede">
      Так часто починається розмова в кабінеті. Зовні все начебто добре — робота, стосунки,
      справи, а всередині — розгубленість, втома чи відчуття, що щось не так,
      і незрозуміло, що саме.
    </p>
    <div class="hero-actions">
      <a class="btn" href="{{ '/kontakty/' | relative_url }}">Записатись на консультацію</a>
    </div>
  </div>
  <figure>
    <img src="{{ '/assets/images/portret-holovna.jpg' | relative_url }}"
         alt="Євген Кочубей, клінічний психолог і гештальт-психотерапевт"
         width="900" height="1350" fetchpriority="high">
  </figure>
</section>

<section class="section" id="shlyakhy">
  <h2>З чим до мене приходять</h2>
  <div class="two-paths">
    <div class="path-card">
      <h3>Чоловіки в кризі</h3>
      <p>
        Зовні все функціонує — кар'єра, бізнес, сім'я, але всередині втома,
        розгубленість, відчуття, що живете не своє життя, труднощі з близькістю.
      </p>
      <p><a href="{{ '/choloviky/' | relative_url }}">Детальніше →</a></p>
    </div>
    <div class="path-card">
      <h3>Тривога, стосунки, самооцінка</h3>
      <p>
        Тривога, яка не минає, апатія, депресія, складнощі в стосунках,
        емоційна залежність, проблеми з самооцінкою та самоцінністю, виснаження
        та вигорання — стани, знайомі багатьом з нас, особливо зараз.
      </p>
      <p><a href="{{ '/zagalni-stany/' | relative_url }}">Детальніше →</a></p>
    </div>
  </div>
</section>

<section class="section-alt">
  <div class="wrap">
    <h2>Самодопомога</h2>
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
  {% include post-cards.html limit=4 %}
  <p><a href="{{ '/blog/' | relative_url }}">Усі статті →</a></p>
</section>

{% include consultation.html %}
