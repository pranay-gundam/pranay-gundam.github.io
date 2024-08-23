---
layout: post
title: few months later... (and spatial econ models)
date: 2023-10-01 11:29:00
description: 

tags: personal-updates econ-thoughts
categories:
disqus_comments: true
---

It’s been a few months now since I’ve moved to NYC and I’ve realized a big issue: having time to think about projects and stuff I want to take on but not having enough time to really thoroughly address everything. So far, I have to deal with a busy time at work, a PhD Macroecon class (that I want to be very diligent about), and bunch of interesting ideas that I really want to do but don’t have enough time for.

One skill that I do want to develop (despite all the things going on above) before I get to grad school is identifying what model/statistical machinery I should used based on the research question that I’m trying to address. We had a seminar speaker come over the other day (he was a postdoc from Harvard who was presenting some paper on the changes in car manufacturing plants due to climate change) and in the RA session afterwards he related this grasp of the econometrics that was very impressive; it’s something I also want to be able to do as well. This is related to my issues with TidyTuesday so far, yes I can do some work on a dataset and make a very simple model to ask some sort of question but it feels very meaningless. There is no great insight, there is no thoughtful model building process, just some really niche dataset that makes it difficult to anything cool. This mindset may just be a byproduct of my current inability to think of cool questions that each dataset would be good to address but it feels like a reverse endeavor. Usually I feel like projects tend to start with questions first and then one tries to find a matching dataset. Maybe its just a matter of looking at TidyTuesday just as it is, an exercise to stay in touch with working with data (one of my econ professors in undergrad described it as going to the gym for working with data). Regardless, I do need to reassess my relationship to TidyTuesday because I actually have quite a few posts in the works but just little motivation to pull through and finish them just due to not really feeling satisfied with what I’m doing (or maybe I’m just doomed to feel like).

The thing that I have been most interested about recently but have yet to been able to work on is a python package for spatial simulations. It’s something I kind of started in the early stages of my undergraduate senior thesis, but I’ve thought a lot more about how to make it more fleshed out. The idea started out with making a map that includes paths of public transportation (kind of like a map of the MTA subway lines). Given this there would be a distribution of N many firms each of which have their own quotas of workers they need stratified by worker “technology” (the term we’ll be using for the skill level of a worker which initially we will only consider to be univariate, aka there is only one type of technology and people’s technology lies on the positive reals; to add more complexity we could consider technology to be some arbitrarily long vector of values where each value in the vector corresponds to a different type of technology). Each of these firms, in addition to having worker requirements are located in some area on the map that we talked about before. The goal of the spatial simulation package, in the very beginning, it to populate workers, each with some random level of technology, and find an optimal location for these workers to locate given some utility functions (which can be in terms of distance to firms, distance to leisure activities, and whatever else where there are separate costs for public transport and non public transport travel) and then visualize how a city could grow. I’m still deciding on whether I should make physical locations a continuum or some discrete choice. This choice really affects the solution to the model; whether or not we can do it analytically or if we have to enlist the use of computational optimization methods.

To make the above setup more precise, there are:

- N many Firms, $$\left\{F_i\right\}^N_{i=1}$$.
- M many Workers, $$\left\{h_i\right\}^M_{i=1}$$.
- In the discrete location case, we define a metric space on a set S of K many locations.
- Each location $S_i$  has certain properties such as population density and availability of leisure activities that may be relevant to the worker’s utility function.

As of now, we’ve fixed the firms location choice problem (something that could be changed in the future) but the worker will solve the maximization problem $$\max_{i,j}u(S_i, F_j)$$.

I’ve thought of a few more places where I can modify the current setup to add more functionality. Features for online vs static equilibrium, visualizing the model, including other analytics, adding a firm optimization problem, and a handful more.

I want to also preface that my knowledge about spatial models is pretty limited. This is just how I would think to setup the problem without having been introduced to any of the literature on the topic.
