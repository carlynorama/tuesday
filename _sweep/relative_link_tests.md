---
layout: default
title: Relative Links Test
showonindexas: link
---

{% for item in site.data.content.relative_link_test.links %}
[{{ item.title }}]({{site.baseurl}}{{ item.support_file }})
{% endfor %}

* [Same dir](sweep_basic_checklist.md)
* [File in learn dir with dots](../_learn/01-news.md)
* [File in learn dir, abs](/_learn/01-news.md)
* [File in learn dir, no leading /](_learn/01-news.md)
* baseurl, FYI: {{ site.baseurl }}