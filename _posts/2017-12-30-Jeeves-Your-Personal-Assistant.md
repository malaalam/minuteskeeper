---
layout: post
title: Jeeves - Your Personal Assistant
---

For a while now, I have been obsessing over Recurrent Neural Networks. I understand them in a superficial, top-level way but would like to dive in and learn more. On a few sporadic occasions, I have pondered if it may be possible to combine my knowledge of audio engineering with deep recurrent neural networks in a hands-on project somehow.

Then a couple of days ago, I came across the [Kaggle](https://www.kaggle.com/c/tensorflow-speech-recognition-challenge) challenge which centred around converting speech to text. While there are [softwares](https://en.wikipedia.org/wiki/Transcription_(software)) in the market which accomplish this, I did not see find many items of hardware **dedicated** to this scope of function. 

That made me envision a device which could generate **minutes of a meeting** for a group of users who are firing ideas at each other. Considering that it is not uncommon to see an employee jot down the minutes by hand in meetings held at corporate offices, suggests to me that *speech to text annotation for official meetings* is a function which could potentially be automated.

The fact that one doesn't hear of such devices already, hints that there might be several, involved technical challenges. I quizzed a friend who has been working in the finance sector for the last three years and he was quick to point out that a good keeper of the minutes is one who (or which) can **eliminate extraneous conversations** and captures the crucial components of the meeting. So that creates a possibility of combining Natural Language Processing (to weed out irrelevant conversations) and Deep Recurrent Neural Networks (for transcribing the audio to text). Another thing the friend mentioned is how when minutes are sent out by emailing, **some context is added** by the *minutes-keeper* so that a reader who wasn't present in the meeting would be able to make sense of the big picture surrounding an intense discussion. That would be an interesting challenge to tackle from the point of view of creating a dedicated automated device - as this implies **content creation** and probably falls (again) in the realm of Natural Language Processing.

Upon some brainstorming with my mother (who usually has some keen insights about most things :O), I realised that another technical challenge would be **tackling multiple conversations at the same time**. I have heard that humans are quite good at [identifying](https://en.wikipedia.org/wiki/Cocktail_party_effect) one source of sound, distinct from another - I wonder how well could a machine separate out two or more sources, and how would these conversations be transcribed (since these occur simultaneously!).

One (more) question which I don't have an answer to is why would a separate hardware be needed for catering to this solution. Would an app suffice, since nowadays phones have quite an impressive processor anyway and can do most of the tasks?

Think there is an opportunity from the point of view of a solving a technical problem. Many companies encourage sending out the minutes to all the concerned employees (just to put in writing all the points which were agreed upon earlier), so if implemented well, this piece of hardware could be used by a large clientele. However, whether these companies would be willing to buy such a product (would such a device justify its cost by improving the productivity of a company) seems hard to answer! .

I thought I would name this project **Jeeves** in reference to the eponymous butler who makes all problems disappear!

<p><figure><a href="http://www.fanpop.com/clubs/jeeves-and-wooster/images/2251468/title/jeeves-wooster-photo"><img src="/images/2017-12-30/jeeves.jpg" alt=""/></a><figcaption>[Jeeves (on the right) and Bertam Wooster]</figcaption></figure></p>





  
