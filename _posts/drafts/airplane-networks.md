---
layout: post
title: airplane networks 
date: 
description: 

tags: econ-thoughts
categories:
disqus_comments: true
---

I have been so unlucky with my flights this year; I haven't had a trip yet where one of the flights wasn't either delayed or canceled. The closest I've got to a perfect trip was just a few weeks ago where my flight got delayed by 15 mins, but everything else has been by either a couple hours or has been a cancellation. For one of my originally planned trip to Dallas, my flight there got canceled and I never got to catch any other flight to Dallas that weekend because of all the people whose flights got canceled and were then on the stand-by list (there were basically around 100 per flight).

This happens to me now mostly because I'm flying from NYC (as opposed to Pittsburgh where the only time I've ever had an issue was once when I was flying to ... you guessed it, NYC). Specifically, NYC (and Atlanta for that matter) are such big airports in terms of air traffic and interconnectivity with other airports that a small weather delay on one side of the country has drastic ripple effects in NYC since there are missing planes or crews. Maybe I've just been at the brunt of a lot of bad luck and we can't design these airport systems any better but maybe there's an interesting question here about how we can do better. Sure there are some unavoidable situations, such as a city being inherently desirable to travel but there are factors that we can control such as how many resources to dedicate to a specific airport or whether or not to connect two airports by a flight path.

I'll go more in detail about how we'll be representing airline traffic networks and the optimization process in the pdf below but to be able to do the optimization we need to make sure we have a well-defined problem. Specifically, we need some framework of characteristics that are *good* and a way to classify one traffic network as being better than another. This is by no means an exhaustive list but here are some characteristics that I've thought of.

- Network A is better than Network B if it costs less.
- Network A is better than Network B if the closing of one or more airports affects fewer flight routes.
- Network A is better than Network B if the average flight path duration is less.

To be able to claim a best network, we have to also come up with some relative weightage for how much we value one of these characteristics over another. I'm not going to make any sort of claim on this here just because that gets into more normative questions about which are more important than others (although I will explore the question in the pdf below).

On one hand, the question of optimizing this network is indeed interesting but I'm also curious about what is the worst that we can do. What would the worst case air traffic network look like? In this case to make sure there is a well-defined problem to solve we have to also craft a unitary definition for the worst network or a class of *bad* characteristics and find networks that have all of them. We can consider it to just be the opposite of the *good* characteristics above, but I'm sure there is another classification that might make more sense based on how we mathematically portray these airline traffic networks.
