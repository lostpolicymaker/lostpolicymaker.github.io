---
layout: acks
title: Lost Policymaker
subtitle: Guide to Villages
use-site-title: true
---

The Hacker Village concept originated with DEF CON as self-contained spaces for specific subject matter, such as lockpicking, cryptography, privacy, and industrial control systems. Many of these have now become non-profit educational organizations that operate year round, offering unique hands-on experiences and presentations. DEF CON 34 features dozens of Villages — the full official list is on the [DEF CON site](https://defcon.org/html/defcon-34/dc-34-villages.html). Several of these may be interesting to the savvy policymaker; if you work in public policy, start with [Policy @ DEF CON](https://defcon.org/policy/).

{% for village in site.data.villages %}

<div class="media">
  {% if village.img %}
  <img src="../img/villages/{{village.img}}" width="64" height="64" class="embed-responsive-item align-self-start mr-3 mt-4" alt="{{village.name}} logo">
  {% endif %}
  <div class="media-body">
    <p><b>{% if village.link %}<a href="{{village.link}}">{{village.name}}</a>{% else %}{{village.name}}{% endif %}</b> <br />
    {{village.description}}</p>
  </div>
</div>

{% endfor %}
