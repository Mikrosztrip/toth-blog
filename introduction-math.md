---
layout: default
title: global.navbar.math
permalink: /math/
navbar_order: 4
navbar_visible: true
---

{%- translate_file pages/math/introduction.md -%}

<!--Extracting documentation pages-->
{% assign documents = site.pages | where: "isDoc", true | sort: "weight" %}
{% assign dir = "math" %}

<!--This will print all documentation hierachy-->
{% include show-children.html dir=dir docs=documents level=2%}

<!--
This will start printing at level 2
{% include show-children.html dir=dir docs=documents level=2 %}

This stop printing at level 2
{% include show-children.html dir=dir docs=documents maxLevel=2 %}
-->