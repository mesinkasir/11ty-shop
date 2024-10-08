---
layout: layouts/page.njk
title: Premium 11ty template
description: Eleventy 11ty premium pro version online shop.
cover: /img/11tyshop.webp
permalink: /premium/
---

<div class="row">
{% for pro in premier %}
<div class="col-md-6 p-3 p-md-5">
<h3><strong>{{pro.title}}</strong></h3>
<p><small>{{pro.description}}</small></p>
<a href="{{pro.url}}" class="btn btn-dark">More info</a>
<a href="{{pro.link}}" class="btn btn-outline-dark">Run Demo</a>
</div>
<div class="col-md-6 p-3">
<img class="img-fluid rounded" alt="{{pro.title}}" width="100%" height="100%" loading="lazy" src="{{pro.cover}}"/>
</div>
{% endfor %}
</div>
{% include "widget/contact.njk" %}
