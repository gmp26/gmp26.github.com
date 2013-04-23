---
layout: post
title: "MathJAX in Jekyll"
description: "Experimenting with GitHub/Jekyll hosted MathJAX"
category: Tech
tags: [MathJAX, Jekyll, Markdown]
---
{% include JB/setup %}

This post is following an [answer on StackOverflow](http://stackoverflow.com/questions/10987992/using-mathjax-with-jekyll).

I've inserted the MathJAX script in \_includes/themes/twitter/default.html. Not yet
sure if this is the optimal place, but it works.

OK - so Markdown has to be kept away from TeX somehow. The solution on Stack Overflow
suggests wrapping with spans or divs. This works, but will be a pain.

Inline with span wrap yields:
<span>\(y=mx+c\)</span>.

Display with div wrap yields: 
<div>\[x=\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}\]</div>

###Notes###
* Currently using backslash parentheses and backslash bracket rather than dollars.
* A double backslash paranthesis gets through Markdown as single backslash parenthesis.
* Double backslash bracket gets interpreted by Markdown as a link.
