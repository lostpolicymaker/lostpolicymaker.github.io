---
layout: acks
title: Lost Policymaker
subtitle: Guide to Villages
use-site-title: true
---

The Hacker Village concept originated with DEF CON as self-contained spaces for specific subject matter, such as lockpicking, cryptography, privacy, and Industrial Controls Systems. Many of these have now become non-profit educational organizations that operate year round, offering unique hands-on experiences and presentations. Several of these may be interesting to the savvy policymaker.

{% for village in site.data.villages %}

<div class="media">
    <img src="../img/villages/{{village.img}}" width="64" height="64" class="embed-responsive-item align-self-start mr-3 mt-4">
<div class="media-body">
<p><b>{{village.name}}</b> <span class="biossocial"><i class="fab fa-twitter"></i> <a href="https://twitter.com/{{village.twitter}}">{{village.twitter}}</a> </span> <br />
{{village.description}} <br /><br />
<em>{{village.quote}}</em></p>
  </div>
</div>

{% endfor %}
