---
layout: page
title: About
permalink: /about/
---

### TLDR;

Hi i'm Paul, Machine Learning Engineer, Founder of the Sydney Machine Learning group & StarAi project lead.

My current focus is on applying Deep Learning to building Strata apartment blocks metering data to detect existing
building services.

Outside of this I actively performing research in the field of Deep Reinforcement Learning for the StarAi project &
 am the Founder of the Sydney Machine Learning group, the largest community of machine learning practitioners in
 Sydney, Australia.

This page contains a brief summary of my work in the field of Machine Learning since I got started back in 2009.
If you would like to know more- read on:

#### In reverse chronological order:

# 2009

### Echo State Networks & Agents : My Introduction to Reinforcement Learning


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
  
<img src="https://media.giphy.com/media/mMCMyT5Q6yvnFyloGi/giphy.gif" data-canonical-src="https://media.giphy
.com/media/mMCMyT5Q6yvnFyloGi/giphy.gif" width="1000" height="500" />

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

### The Years of Doubt.

Take yourself back to the end of 2009. Machine Learning & Ai was not hyped at all. 

In fact, up until 3 years ago (as of
writing this, June 2018), if you mentioned to people that you worked in Artificial Intelligence they would give you this
funny look, then make the same crack joke about the Terminator. 

Point being that there were not many jobs in the 
field,
nor were the existing ones (traders, cough) advertised.

Fresh out of University I headed for the promised land of Australia to seek my fortune. 

I actively practised as a
consulting Electrical Engineer for both [WSP Parsons Brinckerhoff](http://www.wsp-pb.com/wsp-au-nz/) & [Aurecon](https://www.aurecongroup.com/) but 
needless to say, that I was frustrated 
because I could not help seeing how everyday mundane repetitive tasks in engineering might someday be automated with 
Machine Learning. 

I pushed hard for some of my ML ideas to get implemented at these companies, but most people 
laughed &
 no 
one took Machine Learning seriously.

All was not lost however! 

Restlessness caused by knowing how the world would change caused me to travel 
 & see it in a new light. I was lucky enough to visit all of the countries below:

![alt text](https://image.ibb.co/hP0q28/places_Ihave_Been.png)

# 2014 - 2015

### NeuroEvolution: Neural Networks Revisited.

In June 2014 I returned to New Zealand after living in Canada for a year. The first thing I tried to do was get a 
Masters in 
Machine Learning. Again, you have to bare in mind that Machine Learning was not hyped yet. 

The hype was definitely **NOT** real.
 
I went around to 6 different professors at Victoria University, Wellington to try & pitch my idea of using the 
same 
ideas I had developed for my Echo State Network project of 2009 to control a drone.

![alt text](https://image.ibb.co/dvd5kT/Screen_Shot_2018_06_26_at_10_13_47_pm.png)

Drones however, WERE hyped in 2014 and out of the six machine learning professors that I personally approached, none of 
them were 
keen to 
have me on as a masters student. 

No-one had heard of an Echo State State Network and promptly brushed me aside.

I thought, to hell with them, & decided to go [Lone Wolf](https://www.youtube.com/watch?v=l8syGlAMTKA).

From September 2014 to January 2015 I coded up a Neural Network in Java from first principles. 

In 2014 there was no 
fancy [Medium](https://medium.com/@paul.stevhttps://medium.com/@paul.steven.conyngham/how-to-get-blizzard-google-deepminds-pysc2-working-for-free-on-colabs-be2e68f18893) blog posts telling you
 how to do everything, nor were there fancy libraries such as TensorFlow or Pytorch - just a handful of html tutorials
  and of course - 
 research 
papers. 

Everything had to be done from scratch.

I wrote up my Neural Network in Java because I thought that it would be a good way to reteach myself [Object 
Orientated Programmming](https://en.wikipedia.org/wiki/Object-oriented_programming) (OOP - which I learnt at Uni ). I thought this would be a good idea because you can program up
 a neural network in such a way that you could have a Neuron as a separate object, which in then inherited by *a 
 layer of neurons*, which could then be inherited by a "Brain" object. 
 
 The goal of the the Neural Network was to successfully recreate the [XOR function](https://en.wikipedia.org/wiki/XOR_gate) - which was in 2015, the "Hello 
 World" of Machine Learning.
 
 I did *not* however use [Backpropagation](https://en.wikipedia.org/wiki/Backpropagation). 
 
 Instead, [I opted to 
 implement a paper from 1989 "Training Feed Forward 
 Neural Networks via Genetic Algorithms"](https://www.ijcai.org/Proceedings/89-1/Papers/122.pdf). This is the exact 
 same 
 fancy work that [Uber Ai labs proclaimed last year (2017)](https://eng.uber.com/deep-neuroevolution/) as being 
 revolutionary, but ist is actually not that hard 
 core 
 at at 
 all 
 (being a rerun from 1989 and all...). Anyways, I did this because I thought it would be easier to learn, than 
 relearn Partial Derivatives, which I also learnt at Uni -  shout out to [Yann Lecun :) ](https://en.wikipedia.org/wiki/Yann_LeCun#Life) and all the other Electrical
                                                                           Engineers out there!
                                                                           
As you probably guessed, using Genetic Algorithms was a bad idea. Not because Genetic Algorithms are bad per se, but
 because they are an entirely different and unique branch of Machine Learning.  

Having opted to use Genetic Algorithms to train the Neural Networks weights was not a waste of time, as I got to 
learn 
about core 
Genetic Algorithm concepts such as [Fitness Functions](https://en.wikipedia.org/wiki/Fitness_function), [cross-over]
(https://en.wikipedia.org/wiki/Crossover_(genetic_algorithm)) and [mutation rate](https://en.wikipedia.org/wiki/Mutation_(genetic_algorithm)).

I represented the weights of the neural network as the genome, and created  "a population" of different Neural 
Networks, all with different genomes - at the start. Over time, the Neural nets (with weights) that perform the best 
are remembered, whilst the neural nets who perform badly are forgotten. 

The Nets that did well are then "interbred" with other Nets that also performed well, a new population is created, 
and the process is repeated over & over until the Neural Network learned to replicate the XOR function.

[My GitHub Repo for this project is here](https://github.com/PaulConyngham/FFNN-with-genetic-algorithm-training)
                    
# 2016                                
    
### "Concretely."            
                                                                           
                                                                     
 
 
    
 





### Contact me

[paul@sydneymachinelearning.org](mailto:paul@sydneymachinelearning.org)
