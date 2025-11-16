---
layout: default
title: Celebrating the Rich Heritage of Australian Poetry
---

<section class="hero">
  <h2>Celebrating the Rich Heritage of Australian Poetry</h2>
  <p>Explore the poets, stories, and timeless verses that capture Australia’s spirit and identity.</p>
  <p class="cta"><a href="/poems/">Explore Poems</a> <a class="secondary" href="/poets/">Discover Poets</a></p>
</section>

<section class="featured-poets">
  <h3>Featured Poets</h3>
  <ul class="cards">
    {% for poet in site.poets limit:4 %}
      <li class="card">
        <h4><a href="{{ poet.url | relative_url }}">{{ poet.title }}</a></h4>
        <p>{{ poet.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>
</section>

<section class="popular-poems">
  <h3>Popular Poems</h3>
  <ul class="cards">
    {% for poem in site.poems limit:4 %}
      <li class="card">
        <h4><a href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h4>
        <p>{{ poem.excerpt }}</p>
      </li>
    {% endfor %}
  </ul>
</section>

<section class="why">
  <h3>Why Australian Poetry Matters</h3>
  <p>Australian poetry is a living record of the nation — its history, its struggles, and its evolving identity. Explore curated poems, biographies, study resources, and literary analysis.</p>
</section>

<section class="for-sale">
  <h3>Domain For Sale</h3>
  <p>This premium domain — <strong>AustralianPoetry.com</strong> — is available for acquisition. Ideal for arts organisations, educational institutions, and cultural initiatives. <a href="/for-sale/">Learn more & inquire</a>.</p>
</section>
