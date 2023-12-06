---
weight: 10
title: global.math.chapter-1.part-1
---

{% assign documents = site.pages | where: "isDoc", true | sort: "weight" %}
{% assign level = page.dir | remove_first: "/" | split:"/" | size %}
{% assign childrenLevel = level | plus : 1 %}
{% include show-children.html docs=documents dir=page.dir level=childrenLevel %}

{%- translate_file pages/math/chapter-1/part-1.md -%}