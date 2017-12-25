---
layout: page
title: About
description: 代码改变了我
keywords: James Yu, YuJie24
comments: true
menu: 关于
permalink: /about/
---

我是James

我也仰慕「优雅编码的艺术」。

希望能成为一名匠人，静下来写写代码也好。

IF YOU REALLLY WANT IT!

身体力行，live everyday with “Mamba Mentality”！

很惭愧，做的贡献真的太小。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}


### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
