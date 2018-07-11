---
layout: page
title: About
permalink: /about/
---

### TLDR;

Hi i'm Paul, a Machine Learning Engineer, Founder of the Sydney Machine Learning group & StarAi project lead.

I like to employ machine learning methods on novel applications. My current focus is on applying Deep Learning to building Strata apartment blocks metering data to detect existing
building services.

Outside of this I actively performing research in the field of Deep Reinforcement Learning for the StarAi project &
 am the Founder of the Sydney Machine Learning group, the largest community of machine learning practitioners in
 Sydney, Australia.

This page contains a brief summary of my work in the field of Machine Learning since I got started back in 2009.

If you would like to know more, [Follow me on Twitter](https://twitter.com/paul_conyngham) or read on: ;)

#### Contents


- [2009](#2009)
    + [Echo State Networks & Agents : My Introduction to Reinforcement Learning](#echo-state-networks---agents---my-introduction-to-reinforcement-learning)
- [2010 - 2013](#2010---2013)
    + [The Years of Doubt.](#the-years-of-doubt)
- [2014 - 2015](#2014---2015)
    + [NeuroEvolution: Neural Networks Revisited.](#neuroevolution--neural-networks-revisited)
- [2016](#2016)
    + ["Concretely."](#-concretely-)

#### In reverse chronological order:

# 2009

### Echo State Networks & Agents : My Introduction to Reinforcement Learning

[TLDR; The GitHub Repo for my Echo State Network project is here](https://github.com/PaulConyngham/Johnny5_ESN_demo)

I first got started in Machine Learning by being thrown into the "Deep" end with my honours thesis project for my
Electrical Engineering Degree. For this project I used an [Echo State Network (ESN)](http://www.scholarpedia.org/article/Echo_state_network), a type of Neural Network ([Deep Learning](https://en.wikipedia.org/wiki/Deep_learning) for the uninitiated), to
perform control of a virtual agent.

Recurrent Neural Networks (RNNs) are incredibly expensive to train via algorithms such as Backpropagation Through Time
(BTT).

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

[TLDR; The GitHub Repo for my NeuroEvolution project is here](https://github.com/PaulConyngham/FFNN-with-genetic-algorithm-training)

In June 2014 I returned to New Zealand after living in Canada for a year. The first thing I tried to do was get a 
Masters in 
Machine Learning. Again, you have to bare in mind that Machine Learning was not hyped yet. 

The hype was definitely **NOT** real.
 
I went around to 6 different professors at Victoria University, Wellington to try & pitch my idea of using the 
same 
ideas I had developed for my Echo State Network project of 2009 to control a drone.

![alt text](https://image.ibb.co/idqSwo/yeeeehaw.png)

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
Genetic Algorithm concepts such as [Fitness Functions](https://en.wikipedia.org/wiki/Fitness_function), [cross-over](https://en.wikipedia.org/wiki/Crossover_(genetic_algorithm)) and [mutation rate](https://en.wikipedia.org/wiki/Mutation_(genetic_algorithm)).

I represented the weights of the neural network as the genome, and created  "a population" of different Neural 
Networks, all with different genomes - at the start. Over time, the Neural nets (with weights) that perform the best 
are remembered, whilst the neural nets who perform badly are forgotten. 

The Nets that did well are then "interbred" with other Nets that also performed well, a new population is created, 
and the process is repeated over & over until the Neural Network learned to replicate the XOR function.

As one final pass for this project & instead of taking the Object Orientated approach, I recoded the entire thing 
using Linear Algebra (matrices) instead of plain old objects to do everything. This speeding up training time immensely.


                    
# 2016                                
    
### "Concretely."            

[TLDR; the GitHub repo to my MATLAB answers to Andrew Ng's classic machine learning course is here](https://github.com/PaulConyngham/Andrew-NG-Machine-Learning)

[TLDR; the Github repo for my notes on Andrew NGs course are here](https://github.com/PaulConyngham/AndrewNG-MachineLearning-Notes)
                                                                           
The bizarre thing about the NeuroEvolution project was that in 2014-2015, I was just quitley humming away doing 
Machine Learning in my basement (not quite, but you know what I mean). I remember going to a party in 2015 and telling 
people that I was doing machine learning. The girl & her friends that I was talking to at the time gave me quite the 
weird look.

In 2016 however, Machine Learning started to get mentioned in the main stream news. 

This was a new phenomenon, as prior to this Machine Learning was kind of an under ground community.
 
2016 was kind of watershed moment for lets call it "modern Machine Learning" as Deep Learning was now been applied 
to everything & blowing most previously used old school techniques out of the water.

The most famous case of course, being AlphaGo, where the Roger Federer of the "Go" world, Lee Sedol, was beaten by an
 machine learning algorithm/program called [AlphaGo](https://en.wikipedia.org/wiki/AlphaGo). For more info on this 
 there is now an [excellent movie over on Netflix](https://www.netflix.com/title/80190844) about it.
 
I remember being so excited whilst the AlphaGo matches were being played & feeling real sorry for Lee Sedol. He made us all proud in match 4 where he was able to outsmart the algorithm & win one for us Humans. 

AlphaGo was a turning point for many people & I was definitely one of them. I has already decided to make machine learning my life's pursuit-but after watching the AlphaGo-Lee Sedol games I wanted to go further.  
 
I had known about [Andrew Ng's](https://en.wikipedia.org/wiki/Andrew_Ng) now classic course since 2012 & thought that
 it would be a great way to round out my knowledge of the many various other machine learning techniques out there.
 
It was fantastic but extremely painful. For 11 weeks in my spare time after work, all by myself I relearnt Matlab, 
Linear algebra &
 Calculas. Why? You needed to know these topics for the material covered in the course.
 
 In no particular order I got my hands dirty & learnt about: 
 
 Linear Regression, Logistic Regression, Neural Networks (again!), Support Vector Machines, k-Means clustering & principal 
 component analysis (PCA).
 
 The really great thing is that Andrew Ngs course covered the "Supervised Learning" group of Machine Learning techniques. 
 
 Supervised learning, was & still is where the money is at. :)
 
 [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/5ZNJPSe1nZs/0.jpg)](https://www.youtube.com/watch?v=5ZNJPSe1nZs)
 
 Video above: Answers to the Concretely Machine Learning drinking game :)
 
Still being 2016 & after completing Ng's course - the plan I devised was to move to London & try & do something with Machine Learning. I quit my engineering job, bought a ticket & headed off to the UK on a working holiday visa to try out my luck.

I can't quite put my finger on it, but London did not "vibe" with me. It was grey, cold & besides, the machine learning community was already very well established with [DeepMind](https://deepmind.com/) being based there and all.

I had already done a secondment to Sydney in Nov-Dec 2014 for my engineering job & had fallen in love with the place. "trying to do something with machine learning" in London turned out to be not that great of a plan & after spending 3 months in London, on the 1st of January 2017 I headed back to the land of milk & honey, Sydney Australia.

# 2017                                
    
### "The Year of our Lord: Sydney Machine Learning" 

[TLDR; our speed dating analysis app from CS109 is live here:]()

[TLDR; my answers to Harvard Universites CS109 Data Science course is here]()

At the start of 2017, I read Benjamin Frankin's autobiography. In it, I noticed that he set up these little societies wherever he went about the topic he was interested in the most. I thought that this was very interesting. So on the 14th of February I decided to start my own group "Sydney Machine Learning". If I had decided to make machine learning my life's goal, Sydney Machine Learning's purpose would then act a the forcing function to achieve this.

Sydney Machine Learning was like throwing petrol onto a fire & has been insane in terms of accelerating & broading the depth of my knowledge about all things machine learning. I also hope that through my work in the group - that I have given back to the community too.

Setting up SML was no easy endeavour, as any founder will tell you, I faced an insane amount of rejection. 

First, I had to find a venue. I approached many, and faced a ton of rejection. One day in my lunch break however, I decided to catch a train from St James station in central Sydney Sydney to Redfern. Redfern is the home of [Cicada Innovations](http://cicadainnovations.com/), and is Australia's leading high tech accelerator for Startups. I walked into the main foyer, where I met [Marin](https://www.linkedin.com/in/marin-peplinski-2a69013b/), the head of community at Cicada Innovations. I told her what I was trying to do & she said she would speak to her management about it. The next day I received a call from Marin saying that Cicada would be happy to host SML - and with that we has a venue!

We still needed speakers however. Again, I had approached many people and was beginning to run out of ideas. In one final push I decided to email the entire SML group, saying that we were ready to go but still needed speakers. I was lucky enough to have 
 
 
I approached many potential speakers & hosts & got rejected, by all most all. In the process however I got to meet so many interesting people that I would not have otherwise. So in all honesty, the rejection was kind of worth it.
        
            
            
                        
 
 
    
 

From my personal experience, if you are not consistantly learning in the ML field, you will quickly become irrelevant.

I find from experience - to be good at Machine Learning as the field is so vast, you need to be constantly reteaching
 yourself knowledge from all over the field.

### Contact me

[paul@sydneymachinelearning.org](mailto:paul@sydneymachinelearning.org)
