---
layout: post
date: 2019-02-17 23:15:00
title: "testing unless"
category: [tech]
tag: [liquid, test, unless, blog jekyll]
---
Just testing an ```unless``` solution from [SlackOverflow](https://stackoverflow.com/questions/30822160/does-liquid-have-a-does-not-contain-or-not-in-array-operator)

    {% raw %}
    {% assign input = "A,B,C" | split:"," %}
    unless print only if constrain is not met.
    This prints nothing:{% unless input contains 'A' %}No A{% endunless %}
    This prints "No Z": {% unless input contains 'Z' %}No Z{% endunless %}
    {% endraw %}

Gives this output

{% assign input = "A,B,C" | split:"," %}

unless print only if constrain is not met.

This prints nothing:{% unless input contains 'A' %}No A{% endunless %}

This prints "No Z": {% unless input contains 'Z' %}No Z{% endunless %}
