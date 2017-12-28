---
layout: post
title: The Boyer-Moore Algorithm
comments: true
---

While looking for techniques to compare one short strand of DNA with a reference genome, I came across the Boyer-Moore Algorithm. First discussed in [1977](http://www.cs.utexas.edu/users/moore/publications/fstrpos.pdf), it suggested a rather intuitive approach to scan a large text for a pattern. While the *Naive Exact Matching* considers the pattern as a template and moves it along the length of the text - from left to right - one letter at a time, the Boyer-Moore approach relies on two heuristics - *Bad Character* and *Good Suffix* - to skip some of the comparisons. 

Here is an excerpt from a recent [publication](http://www.cs.utexas.edu/users/moore/publications/sustik-moore.pdf) by Sustik and Moore, where they state that in situations when pre-processing can not be done, maybe because the reference text changes quite frequently (within genomics, the text - say the reference genome - does not change too often, so other offline techniques are probably used more), the algorithm is a good choice:

> "The Boyer-Moore algorithm and its variants perform best when preprocessing of the text is not possible or not desired. The search is linear in the size of the text, and in fact it has been shown that no character needs to be read (and compared) more than three times. Subsequent variants guarantee at most 2n comparisons for a text consisting of n characters"

As an example, consider the text T and pattern P in the slide below  (taken from Dr. Ben Langmead's lectures). Here the pattern is aligned with the text, the Bad Character and Good Suffix Rules are applied and the maximum of the two predictions is taken to shift the pattern further down towards the right. 

<p><figure><a href="https://github.com/BenLangmead/ads1-slides"><img src="/images/2017-12-16/Boyer-Moore2.JPG" alt=""/></a><figcaption>
   [Applying Bad  Character (bc) and Good Suffix (gs) Rules to determine how many letters in the text (T) can be skipped during comparison with pattern (P) using the Boyer-Moore Algorithm.]</figcaption></figure></p>

I wonder if this algorithm is used nowadays in analysing genomics - is there any scenario, for example, where its use is preferred over that of hash tables? 