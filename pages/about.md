---
layout: page
title: About
description: Taotao'blog
keywords: Taotao
comments: true
menu: 关于
permalink: /about/
---

# 生命不息，折腾不止 #

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}


{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}