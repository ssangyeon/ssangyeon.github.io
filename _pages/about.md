---
permalink: /
title: "Sangyeon Yoon"
excerpt: "Researching reliability, unlearning, and evaluation for large language models."
layout: splash
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}
{% assign selected_papers = site.data.publications | where: "selected", true %}
{% assign total_outputs = site.data.publications | size %}

<div class="home-shell">
  <section class="home-hero" id="top">
    <div class="home-grid home-hero__layout">
      <div class="home-hero__content">
        <p class="home-kicker">M.S. Student in AI at Yonsei University</p>
        <h1 class="home-hero__title">
          Building more <span>reliable</span> language models for the real world.
        </h1>
        <p class="home-hero__lead">
          I study robustness, evaluation, and unlearning in large language models,
          with a focus on hidden failure modes, realistic risk, and trustworthy deployment.
        </p>
        <div class="home-hero__chips" aria-label="Research topics">
          <span>LLM Reliability</span>
          <span>Robust Evaluation</span>
          <span>Machine Unlearning</span>
          <span>Reasoning Behavior</span>
        </div>
        <div class="home-hero__actions">
          <a class="btn btn--primary" href="{{ base_path }}/publications/">View Publications</a>
          <a class="btn btn--inverse" href="{{ site.author.googlescholar }}">Google Scholar</a>
          <a class="btn btn--light-outline" href="https://github.com/{{ site.author.github }}">GitHub</a>
        </div>
      </div>

      <aside class="home-hero__card">
        <div class="home-portrait">
          <img src="{{ base_path }}/images/profile3.png" alt="Portrait of Sangyeon Yoon"/>
        </div>
        <p class="home-hero__eyebrow">Currently</p>
        <h2>Researching LLM reliability at Yonsei University.</h2>
        <p>
          Advised by Prof. Albert No, and recently worked as a research intern
          at EXAONE Lab, LG AI Research.
        </p>
        <dl class="home-facts">
          <div>
            <dt>{{ total_outputs }}</dt>
            <dd>research outputs listed</dd>
          </div>
          <div>
            <dt>ICLR 2026</dt>
            <dd>latest accepted venue</dd>
          </div>
          <div>
            <dt>EXAONE Lab</dt>
            <dd>recent industry research experience</dd>
          </div>
        </dl>
      </aside>
    </div>
  </section>

  <section class="home-metrics">
    <div class="home-grid home-metrics__grid">
      <article class="home-metric">
        <p class="home-metric__label">Research lens</p>
        <p>How do language models fail outside neat benchmark settings?</p>
      </article>
      <article class="home-metric">
        <p class="home-metric__label">Recent venues</p>
        <p>ICLR 2026, EMNLP 2025 Main, NeurIPS 2025, and NeurIPS 2024 SFLLM.</p>
      </article>
      <article class="home-metric">
        <p class="home-metric__label">Core themes</p>
        <p>Evaluation, robustness, reasoning, personalization, and machine unlearning.</p>
      </article>
    </div>
  </section>

  <section class="home-section" id="research">
    <div class="home-section__inner">
      <div class="home-section__heading">
        <p class="home-kicker">Research</p>
        <h2>What I work on</h2>
        <p class="home-section__body">
          My work sits at the intersection of evaluation, reliability, and model behavior.
          I try to find the gap between what benchmarks say and how foundation models act in practice.
        </p>
      </div>

      <div class="home-card-grid">
        <article class="focus-card">
          <p class="focus-card__index">01</p>
          <h3>Reliability beyond benchmark averages</h3>
          <p>
            I design evaluations that surface hidden behaviors, long-tail failures,
            and deployment risks that standard benchmarks often smooth over.
          </p>
          <div class="home-tag-list">
            <span>Robustness</span>
            <span>Benchmarks</span>
            <span>Failure Analysis</span>
          </div>
        </article>

        <article class="focus-card">
          <p class="focus-card__index">02</p>
          <h3>Understanding what LLMs retain and forget</h3>
          <p>
            I study machine unlearning, knowledge separation, and reasoning traces
            to understand how models absorb, preserve, and discard information.
          </p>
          <div class="home-tag-list">
            <span>Unlearning</span>
            <span>Knowledge Use</span>
            <span>Reasoning</span>
          </div>
        </article>

        <article class="focus-card">
          <p class="focus-card__index">03</p>
          <h3>Making evaluation more realistic and personalized</h3>
          <p>
            I am interested in context-aware evaluation settings that better reflect
            real user preferences, memory, and the messiness of real deployment.
          </p>
          <div class="home-tag-list">
            <span>Personalization</span>
            <span>Persistent Memory</span>
            <span>Practical Safety</span>
          </div>
        </article>
      </div>
    </div>
  </section>

  <section class="home-section home-section--tinted" id="highlights">
    <div class="home-section__inner">
      <div class="home-section__heading">
        <p class="home-kicker">Highlights</p>
        <h2>Recent momentum</h2>
        <p class="home-section__body">
          A snapshot of the last year across publications and research experience.
        </p>
      </div>

      <div class="timeline-grid">
        <article class="timeline-card">
          <p class="timeline-card__date">Jan 2026</p>
          <h3>Two papers accepted to ICLR 2026</h3>
          <p>Recent work on unlearning failures and safety alignment for diffusion language models.</p>
        </article>

        <article class="timeline-card">
          <p class="timeline-card__date">Sep 2025</p>
          <h3>Joined EXAONE Lab at LG AI Research</h3>
          <p>Worked as a research intern on foundation-model reliability and related evaluation problems.</p>
        </article>

        <article class="timeline-card">
          <p class="timeline-card__date">Aug 2025</p>
          <h3>Two papers accepted to EMNLP 2025 Main</h3>
          <p>Research spanning machine unlearning in large reasoning models and robust separability measures.</p>
        </article>

        <article class="timeline-card">
          <p class="timeline-card__date">Dec 2024</p>
          <h3>NeurIPS 2024 SFLLM Workshop paper</h3>
          <p>Presented work on tighter privacy auditing under final model-only scenarios.</p>
        </article>
      </div>
    </div>
  </section>

  <section class="home-section" id="papers">
    <div class="home-section__inner">
      <div class="home-section__heading">
        <p class="home-kicker">Selected Work</p>
        <h2>Featured papers</h2>
        <p class="home-section__body">
          A few papers that best represent the direction of my recent work.
        </p>
      </div>

      <div class="paper-showcase">
        {% for paper in selected_papers limit: 4 %}
          <article class="paper-card">
            <p class="paper-card__meta">
              {{ paper.venue }}
              {% if paper.status and paper.status != "" %}
                / {{ paper.status }}
              {% endif %}
              / {{ paper.year }}
            </p>
            <h3>
              <a href="{{ paper.pdf_url }}">{{ paper.title }}</a>
            </h3>
            <p class="paper-card__authors">{{ paper.authors }}</p>
          </article>
        {% endfor %}
      </div>

      <div class="home-section__footer">
        <a class="home-text-link" href="{{ base_path }}/publications/">
          Browse the full publications list
          <span aria-hidden="true">&rarr;</span>
        </a>
      </div>
    </div>
  </section>

  <section class="home-section home-section--tinted home-section--last" id="contact">
    <div class="home-section__inner">
      <div class="home-section__heading">
        <p class="home-kicker">Contact</p>
        <h2>Academic depth with an industry view</h2>
        <p class="home-section__body">
          I like working on questions where rigorous evaluation meets practical model behavior.
        </p>
      </div>

      <div class="experience-grid">
        <article class="experience-card">
          <p class="experience-card__meta">Yonsei University</p>
          <h3>M.S. Student in Artificial Intelligence</h3>
          <p>
            Studying large language models with a focus on reliability, evaluation,
            and the ways benchmark performance can miss real-world behavior.
          </p>
        </article>

        <article class="experience-card">
          <p class="experience-card__meta">LG AI Research</p>
          <h3>Research Intern, EXAONE Lab</h3>
          <p>
            Worked on foundation-model research in an industry setting, bringing a product-facing
            perspective to safety, evaluation, and model understanding.
          </p>
        </article>

        <article class="contact-card">
          <p class="experience-card__meta">Connect</p>
          <h3>Find the work</h3>
          <p>For papers, code, and updates, these are the best starting points.</p>
          <div class="home-link-stack">
            <a href="{{ site.author.googlescholar }}">
              <span>Google Scholar</span>
              <strong>Publications</strong>
            </a>
            <a href="https://github.com/{{ site.author.github }}">
              <span>GitHub</span>
              <strong>@{{ site.author.github }}</strong>
            </a>
            <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}">
              <span>LinkedIn</span>
              <strong>{{ site.author.name }}</strong>
            </a>
          </div>
        </article>
      </div>
    </div>
  </section>
</div>
