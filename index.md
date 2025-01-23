`---
title: Yong-Woo Lee
---

# Yong-Woo Lee / 이용우 / 李鎔宇

Welcome! I am a PhD student studying in the Department of Mathematical Sciences in Seoul National University, advised by [Sung-Soo Byun](https://sites.google.com/view/sungsoobyun/welcome). I am interested in probability theory and complex analysis, especially on random matrix theory.

I am a student member of [SNU Probability Group](https://sites.google.com/view/snuprob/).

## Publication
<ol>
  {% for publication in site.data.publications %}
    <li>
      <strong>{{ publication.title }}</strong>, <em>{{ publication.journal }}</em> ({{ publication.year }}) <br>
      Authors: {{ publication.authors }}, <a href="{{ publication.link }}" target="_blank">[Journal Link]</a>,
      {% if publication.arxiv %}
        <a href="{{ publication.arxiv }}" target="_blank">[arXiv Link]</a>
      {% endif %}
    </li>
  {% endfor %}
</ol>

## Talks and Posters
<ol>
  {% for talk in site.data.talks %}
    <li>
      {% if talk.type == "poster" %} <strong>(Poster)</strong> () {% endif %} {{ talk.title }}, {{ talk.location }},
      {% if talk.link %}
        <a href="{{ talk.link }}" target="_blank">[More Info]</a>
      {% endif %}
    </li>
  {% endfor %}
</ol>

<p>Last updated: {{ date: '%Y-%m-%d' }}</p>
