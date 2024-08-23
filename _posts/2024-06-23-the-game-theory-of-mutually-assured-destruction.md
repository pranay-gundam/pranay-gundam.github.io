---
layout: post
title: the game theory of mutually assured destruction
date: 2024-06-23 21:36:00
description: Note, Some spoilers for the Remembrance of Earth's Past series

tags: econ-thoughts
categories:
disqus_comments: true
---

I have been getting a lot of ideas/questions from the Remembrance of Earth's Past series. One of the concepts that shows up towards the end of the second book, The Dark Forest, and is discussed in a lot more detail in the third book, Death's End, is the deterrence through mutually assured destruction or MAD.

One quick tangent: I searched up what exactly the definition of MAD entails and although the definition of the terminology itself should apply, the term itself in the context of what it was made for applies specifically to mutually assured destruction through nuclear weapons with a first strike against a nation with second strike capabilities. So I'm not super sure if MAD the best term to describe what was happening in Death's End since it was only one side threatening the destruction of both parties, in the book they call it simply "Dark Forest Deterrence" but for the sake of this post I'll continue to call it MAD just because it does have logical parallels to the origin of the term (and also MAD is fewer characters to type out each time)

In the book, the way MAD was threatened was through an "universal broadcast" that Earth could send out that included the located of the alien species' star system and since humankind's system and Trisolaris' system were so close together that this would cause other alien species to discover the solar system as well. The reason why discovery was so scary was because this series ascribes to the "Dark Forest" explanation as to why alien civilizations were so hard to find: that all the surviving civilizations were very technologically advanced groups who distrusted every other civilization by default and operated under a "shoot on sight" protocol so broadcasting one's location would get them immediately annihilated. In the case of Earth, this broadcast system was under control of a single individual. This, of course, was an immense responsibility since they were in control of the fate of two civilizations. So, in picking who that individual would be, one would have to make sure that it would be a person who would not activate the signal needlessly, but also give the impression that they would activate the signal when being attacked.

This is a very similar issue to what the US had faced during the Cold War. Whenever I watch documentaries or listen to podcasts on the subject, they always talk about how there was so much research being done on this MAD-related game theory problem. For most of my life prior, I always thought that this was really silly given that my impression was that game theory was one of those simple 2x2 games. In retrospect now, I realize that to truly model the complexity of what is going on and include more nuances specific to the situation, you have to consider the exact mechanisms by which a MAD situation would be activated. Questions such as: who exactly has control of the launch, are they likely to retaliate even if they already know they are doomed, are there multiple people involved in the launching of nuclear weapons, how do you maximize the perception of one's threat against their opponent without sacrificing other things? All these are questions that can be incorporated into a model that make the question a bit more interesting than one of those "2x2 Find the Nash Equilibria" games.

I'll detail one such model soon, but just for some context we can make to the archetypical 2x2 we see in high school Econ classes (note: that most of these changes are taken as part of a standard model in game theory in the literature, I'm not too read up on it so I may be missing a few key components):

- Tack on some functional structure for the probabilities that both the first and second strike of MAD are activated.
- Introduce multiple actions (with complete destruction being minus infinity utility). One can even make it an action that lies on some continuous domain instead of discrete choices.
- For games with sequential actions, we can represent the problem as nested games with each action taken further filtering the state spacetakes.

With all that in mind, let's try to construct a model for a Cold War-type situation between two world powers.
