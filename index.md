---
title: Yong-Woo Lee
---

# Yong-Woo Lee / 이용우 / 李鎔宇

Welcome! I am a PhD student studying in the Department of Mathematical Sciences in Seoul National University, advised by [Sung-Soo Byun](https://sites.google.com/view/sungsoobyun/welcome). I am interested in probability theory and complex analysis, especially on random matrix theory.

I am a student member of [SNU Probability Group](https://sites.google.com/view/snuprob/).

## Publication
<ul>
  {% for publication in site.data.publications %}
    <li>
      <strong>{{ publication.title }}</strong>, <em>{{ publication.journal }}</em> ({{ publication.year }}), 
      <a href="{{ publication.link }}" target="_blank">[Journal Link]</a>
      {% if publication.arxiv %}<a href="{{ publication.arxiv }}" target="_blank">[arXiv Link]</a>{% endif %}
      <br>Authors: {{ publication.authors }}
    </li>
  {% endfor %}
</ul>

## Talks and Posters
<ul>
  {% for talk in site.data.talks %}
    <li>
      <strong>{{ talk.title }}</strong>, {{ talk.title }} <br>
      Location: {{ talk.location }} <br>
      Date: {{ talk.date }} <br>
      {% if talk.link %}
        <a href="{{ talk.link }}" target="_blank">[More Info]</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>

<p>Last updated: {{ date: '%Y-%m-%d' }}</p>
