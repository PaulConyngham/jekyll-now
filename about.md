---
layout: page
title: About
permalink: /about/
---

### TLDR;

Hi i'm Paul, Machine Learning Engineer, StarAi project lead & founder of the Sydney Machine Learning group.

My current focus is on applying Deep Learning to building Strata apartment blocks metering data to detect existing
building services.

Outside of this I actively performing research in the field of Deep Reinforcement Learning for the StarAi project &
 am the lead organizer of the Sydney Machine Learning group, the largest community of machine learning practitioners in
 Sydney, Australia.

This page contains a brief summary of my work in the field of Machine Learning since I got started back in 2009.
If you would like to know more- read on:

#### In reverse chronological order:

# 2009

### Echo State Networks & Agents : My Introduction to Reinforcement Learning

![Johnny5](https://media.giphy.com/media/mMCMyT5Q6yvnFyloGi/giphy.gif)


I first got started in Machine Learning by being thrown into the "Deep" end with my honours thesis project for my
Electrical Engineering Degree. For this project I used an [Echo State Network (ESN)](http://www.scholarpedia
.org/article/Echo_state_network), a type of Neural Network ([Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) for the uninitiated), to
perform control of a virtual agent.

Recurrent Neural Networks (RNNs) are incredibly expensive to train via algorithms such as Backpropagation Through Time
(BTT)
.

Echo State Networks (ESNs) are a form of Recurrent Neural Networks (RNNs) developed to address the incredible
 "training" difficulty of vanilla RNNs- by having a fixed "reservoir" of randomly connected layers of virtual neurons, and
  a final "trainable" layer that connects to the "reservoir". Echo State Networks fall under the research branch of
  ["Liquid State Machines"](https://en.wikipedia.org/wiki/Liquid_state_machine), a genre of Neural network that is known within research communities to closely match the
  functionality of real neural networks of the human brain.

The goal of this research project was to have an autonomous "agent" navigate to a random point in 2D space. Once it
reached the goal, the navigation point was reset and the agent would have to start over. By resetting the "final
destination" like this, we were able to demonstrate that the agent was actually learning.

Back in 2009, there were no fancy libraries like Pytorch & Tensorflow and I personally coded up the navigation
environment in pure C, and used ESN classes written by my supervisor, [Dr Russell Webb](https://www.linkedin.com/in/russ-webb-52a164/).

In the video above, we can see the agent attempting to navigate to target point in space denoted by an X. The agent is
represented by a simple arrow (to show the direction it is currently pointing).

Continuing to code up the
entire machine learning project in C, I wrote up my own Reinforcment Learning Framework to wrap the ESN classes provided
 by my supervisor such that the "reward signal" was the distance that the agent was away from the "X". Training was
 achieved by instantiating two copies of the ESN Agent with slightly modified versions of the last layer of the ESN's
 network. The copy of the ESN agents network that produced a higher reward was remembered, whilst the other was
 forgotten. This framework produced surprising results, most notably, the agent learning to navigate to the point in 2D
 space.

Personally, I could not believe the result -  as no "hard rules" had been programmed into the system
other than the agent had access to the actions of moving left, right and accelerating in the direction it was currently
pointing. What this meant is that the network had been able to infer some form of the "laws of motion" or pythagorean
vectorization - all on its own. From this point on - I was hooked on machine learning.

# 2010 - 2013

### The Golden Years :)

Take yourself back to the end of 2009. Machine Learning & Ai was not hyped at all. Infact up until 3 years ago (as of
writing this June 2018), if you mentioned to people that you worked on artificial intelligence they would give you this
funny look, then make the same crack joke about terminator. Point being was that there were not many jobs in the field,
nor were the existing ones (traders, cough) advertised.

Fresh out of University I headed for the promised land of Australia to seek my fortune. I actively practised as an
consulting Electrical Engineer for both Parsons Brinckerhoff & Aurecon but needless to say, that I could not help seeing
  how everyday mundane repetitive tasks done in this field might someday be automated with machine learning.



### Contact me

[sydneymachinelearning@gmail.com](mailto:sydneymachinelearning@gmail.com)
