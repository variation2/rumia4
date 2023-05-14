+++
author = "Rumia"
date = "2023-03-20T13:56:01-08:00"
meta = true
math = true
title = "Computational Neuroscience Is a Fool's Errand"
toc = true
categories = ["ai", "ml", "neuro", "physics"]


+++

## Introduction

We're in the midst of an AI spring blooming so vividly that only the most cynical haven't hopped onto this train of hope for the future, the hope that one will be a part of creating something special, something that will change the world. 

Two things, both equally as alarming to me, urged me to write this essay. A few weeks prior, I was discussing the future of AI with some of the world's best machine learning researchers. There has been a question that I thought would be lurking in everyone's mind in the past months of if it is possible to align a strong AI, AGI, with the powers of a weaker one. I don't even see how anyone could saliently respond "yes" to that question, but they did. Unfortunately, everyone is so excited about the possible advent of AGI that they've thrown ethics out the window. They also told me that AGI will be here in the next ten to fifteen years.

That is a bold prophecy, but it's not an uncommon belief at all. A friend of mine has grand plans of making his fortune in the field of computational neuroscience in the hope that it will lead to AGI. The classical argument against the viability and even practicality of mathematical modelling of the brain (which I'll refer to to as "modelling" from now on) has always been - not enough compute. I've always told these people, "If you want to model a brain, go to quantum computing and stop bothering neuroscientists," but I've now realized that the problem of not enough compute is so unexpectedly massive that - it's impossible even with a quantum *deus ex machina*. 

First, some easily negated premises that I include for completedness despite their tangentiality. There is an incorrect assumption that modelling is as easy as cobbling together many neural networks of different types (mimicking different areas of neurons and their basic propagation patterns). This is as naive as a young child thinking all of mathematics is additive. In simplest terms, a real brain is at least a directed, weakly connected graph of neurons, and the number of those "weak" connections is not small by any means. Besides, the current research on propagation patterns of neurons is feeble, and I have my personal doubts about action potentials being the only form of signal propagation. 

I also need to point out the conveniently ignored fact that the brain is only part of the central nervous system, and to our knowledge doesn't have any sensory neurons of its own. (I've heard of a case now where there *was* sensation in the brain, but this seems to be reserved for a rare few.) I won't even discuss motor neurons here because the challenge they pose is nightmarishly outside of the scope of our initial goal, learning. Regardless, there are only a few paths for input, and it's still an open problem of how to mimic real sensory input, as this will be the only input to the neural network. Take the human eye, of which the sensory cells of the retina are actually neurons. A single photon falling onto the retina is absorbed by a single molecule of rhodopsin, quickly the neuron is depolarized, and an action potential propagates. Here our main problem comes to light for the first time. 

A photon's energy is given by $E = \frac{he}{\lambda}$ where $\lambda$ is the wavelength, and $c$ and $h$ are the speed of light and the Planck constant, respectively. Now, humans supposedly see in the range of 380 to 700 nm, so the energy of our absorbed photon is as small as $2.837779^{-28}$ joules. Meanwhile, an action potential has $3.05^{12}$ joules of energy. The assumption of using action potentials as quantums crumbles instantly. It was already a weak idea due to there being different sizes of potentials that are summative, but they are usually measured in mV, so computing at the accuracy of membrane potentials in mV is unrealistic. The idea of using quantums to represent something as small as a photon is ridiculous because a photon itself is already a quantum. To sufficiently represent visual input, we need $1.5038806^{25}$ times more energy (for modellers, that's multitudes of memory) than previously assumed. The question of how energy was so amplified also stands, and cannot be simulated until it is known. The answer is hidden in plain sight, in our cells. But never *in silico*. 