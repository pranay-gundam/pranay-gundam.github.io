---
layout: post
title: the dynamics of incumbent politicians pt. 2
date: 
description: 

tags: econ-thoughts
categories:
disqus_comments: true
---

The first thing I need to do is preface some addundum in the jupyter file below. The number of oversights one makes when the only thing editing is an AI gives me a bit of hope that it won't steal *all* of our jobs. There's not anything neccesarily wrong per say with the model I discussed last week but I really skimmed over a few details. First, the model I defined last week is a little bit different than the canonical job search question in that we have stochastic transitions and the politician's choices affect this transition as well.

One other technique I forgot to mention (that I haven't really seen in the econ literature/classes but is a pretty relevant method in reinforcement learning in ML) is Q-learning.

{% raw %}

```liquid
{::nomarkdown}
{% assign jupyter_path = 'assets/jupyter/incumbent-politicians.ipynb' | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/incumbent-politicians.ipynb %}{% endcapture %}
{% if notebook_exists == 'true' %}
  {% jupyter_notebook jupyter_path %}
{% else %}
  <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
```

{% endraw %}
