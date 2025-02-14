---
layout: post
title: the dynamics of incumbent politicians pt. 2
date: 
description: 

tags: econ-thoughts
categories:
disqus_comments: true
---
This post is the long awaited (at least for myself) pt. 2 for the post [*the dynamics of incument politicians pt. 1*](https://pranay-gundam.github.io/blog/2024/dynamics-of-politicians/). It picks off on the model from last time by actually implementing it and creating a few visuals to look at to get a better sense of how we could look at the incentive structure of politicians from one strategy that economists would use to analyze the question.

Now with that said the first thing I need to do tack on some addundum from part one of this post. The number of oversights one makes when the only thing editing is an AI gives me a bit of hope that it won't steal *all* of our jobs. There's not anything neccesarily wrong per say with the model I discussed in part one but I really skimmed over some important details. First, the model I defined last in part one is a little bit different than the canonical job search question in that we have stochastic transitions and the politician's choices affect this transition as well. Second, I definitely should have made the problems regarding the size of the policy space abundantly clear: I went for an ambitious model where the politician has a lot of choices of what they can do in each time, I'm trying to retain these choices but in doing so I have to sacrifice the extent to which the politican can consider each choice for the sake of having my code run in reasonable time.

One other technique I forgot to mention (that I haven't really seen in the econ literature/classes but is a pretty relevant method for reinforcement learning in ML) is Q-learning. This is a method that is very applicable in the scenario that I am discussing right now and I haven't yet seen (although I am near positive that they exist) any problems in macro with stochastic transisions that depend on the action that the agent takes. In this case the politician's transition probabilities into become elected in or "elected out" is itself dependent on both how much they spend on the elected and how they vote. For now, I did the value iteration by considering the expected value of the transition probability, but I'm also going to implement a Q-Learning thing as well just to see if they converge to the same value/policies (and for practice).
