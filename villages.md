---
layout: acks
title: Lost Policymaker
subtitle: Guide to Villages
use-site-title: true
---

The Hacker Village concept originated with DEF CON as self-contained spaces for specific subject matter, such as lockpicking, cryptography, privacy, and industrial control systems. Many of these have now become non-profit educational organizations that operate year round, offering unique hands-on experiences and presentations. DEF CON 34 features nearly forty Villages — far too many to see in a weekend — so below are the ones the savvy policymaker is most likely to find useful, roughly in that order. Often the fastest way to understand a policy issue is to walk in and put your hands on it. The [full official roster](https://defcon.org/html/defcon-34/dc-34-villages.html) has the rest.

{% for village in site.data.villages %}

<div class="d-flex">
  {% if village.img %}
  <img src="../img/villages/{{village.img}}" width="64" height="64" class="align-self-start me-3 mt-4" alt="{{village.name}} logo">
  {% endif %}
  <div class="flex-grow-1">
    <p><b>{% if village.link %}<a href="{{village.link}}">{{village.name}}</a>{% else %}{{village.name}}{% endif %}</b> <br />
    {{village.description}}</p>
  </div>
</div>

{% endfor %}
