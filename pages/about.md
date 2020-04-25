---
layout: page
title: About
description: 星际工作室
keywords: 星际工作室
comments: true
menu: 关于
permalink: /about/
---

星际工作室

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
</li>
{% endif %}
</ul>



## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}

<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
