---
layout: post
title: The Age of Perceptron
categories: deepLearning
tags: Rosenblatt, Minsky, Pappert
comments: true
---

A lot of texts on machine learning hark back to the time when the perceptron algorithm was initially discovered. Popularized by Frank Rosenblatt and expounded in his book [Principles of neurodynamics. Perceptrons and the theory of brain mechanisms](https://scholar.google.com/scholar_lookup?title=Principles%20of%20neurodynamics%3A%20Perceptions%20and%20the%20theory%20of%20brain%20mechanism&author=F.%20Rosenblatt&publication_year=1961), it described a binary classifier which could assign linearly, separable input vectors to their individual classes. The algorithm gripped the attention of the masses and attracted a very similar debate on the merits and de-merits of Artifical Intelligence, as is probably happening now. Several claims of success at delineating two classes of objects were made, which were negated in a text by Minsky and Pappert. I found this interesting on two fronts: First of all, Rosenblatt and Minsky grew up in the same neighbourhood, studied different professions and realized their interest lay in the realm of artificial intelligence but would eventually end up taking contrasting views. I wonder how the volley and rebuttal of claims happened betweeen the two at that time, and if it ever became vitriolic (I discovered that before his early death, Rosenblatt acknowledged the positive contribution of Minsky in taking the field forward - so they made peace in time perhaps!). Second, just as with the successes of Deep Learning now, the Perceptron Algorithm had a massive fan following which came crashing down after Minsky stated that many of the things it claimed to do were untrue. This lead to a cooling off of public gaze and flow of research funds into the field, until its revival again in the 1980s.

<p><figure><a href="http://tfwiki.net/wiki/Perceptor_(G1)"><img src="/images/2017-12-23/perceptor.jpg" alt=""/></a><figcaption>
   [Perceptor from Transformers: Was the name of the character inspired by the similar-sounding algorithm? :)]</figcaption></figure></p>

Rosenball's opus makes a fascinating and lucid read. The author mentioned in the preface, how he requested well-meaning popularizers to suppress their urge to capitalize the letter *P* in perceptron, as it gave the false impression that it was a piece of hardware, instead of an algorithm. 

>"On being asked "How is Perceptron performing today?" I am often tempted to respond, "Very well, thank you, and how are Neutron and Electron behaving?"
 
Rosenblatt seemed to be interested in the problem of memory storage and was working on finding a model that explained the *distributed memory* and *equipotentiality* as discovered by Karl Lashley through his experiments on rats. That made me curious to know more about Lashley's experiments (In order to understand if memory is localized in a certain portion of the brain, Lashley induced lesions on rats' brains and evaluated any differences in ability to cross a maze **before and after** being subjected to this injury). Here is a paragraph from one of [Lashley](http://psychclassics.yorku.ca/Lashley/neural.htm) 's texts:

>"Let us turn now to another important aspect of cerebral function. A review of symptoms suggests that no logically derived element of behavior can be shown to have a definite localization; no single sensation, memory, or skilled movement is destroyed alone by any lesion. On the contrary the various parts of the functional areas seem equipotential for such elements, and either a whole constellation of them is affected by the lesion, or none at all."

Makes me realize that I do not know much about the various physiological features and models to explain memory allocation associated with the brain! Also, is there any evolution-based reason why we have multiple lobes related to different brain functions, since if each lobe is capable of processing any kind of sensory information and retaining elements of behaviour, a single lobe would have been enough! (Are there any anatomical differences between lobes?)   



