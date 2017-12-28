---
layout: post
title: Splattering your RNA away
comments: true
---

I earned a post-graduate degree in applied mechanics. For several years henceforth, I juggled with acoustics and fluid dynamics in industry. Then one warm, dusty afternoon, I came across the [opus on genetics](https://en.wikipedia.org/wiki/The_Gene:_An_Intimate_History) written by Dr. Siddharth Mukherjee. I ploughed through it, reading it in around two days and suddenly I was smitten by the idea of combining data science with genetics. I remember pacing across my apartment trying to grapple with some of the concepts mentioned in the book. That any two people are *99.9 %* alike in their genemaps and yet we all look so different amazed me (I thought the difference could have been more!); that a FastQ file containing the complete human genome would be around [200 GB large](https://medium.com/precision-medicine/how-big-is-the-human-genome-e90caa3409b0) suggested to me the *bigness* of data we are dealing with; that in the future, we would be able to extrapolate one's facial characteristics based on one's genemap seemed a [startling idea](https://www.technologyreview.com/s/608813/does-your-genome-predict-your-face-not-quite-yet/).

To me, the field of genomics seemed suitable for the application of machine learning. I was intrigued about the possibility of combining the two and scoured some of the existing works at their intersection - but realized quickly enough, that I would need some education in both these fields before I can be useful.

To kick-start my journey in genomics, I joined Debarka [Sengupta's lab](https://www.iiitd.ac.in/debarka). Here, we build methods to analyse data obtained from single cell RNA - sequencing (scRNA-seq) Techniques. As I have understood, scRNA-sequencing came to the fore only recently - maybe in around 2012-13. The plummeting cost of sequencing has made it economically feasible to apply at a more discrete level than bulk-cell data. In principle, once the methods of analysis around scRNA are established, there would be a better understanding of cell differentiation, proliferation and signaling. However, scRNA sequencing comes with a *disadvantage* that gene-wise contributions become more sparse - which results in a high frequency of negligible read counts for certain genes (called as *technical drop-outs*).  

<p><figure><a href="https://hemberg-lab.github.io/scRNA.seq.course/differential-expression-de-analysis.html#single-cell-rna-seq"><img src="/images/2017-12-10/zeroInflation.png" alt=""/></a><figcaption>
   [High number of zero read counts in scRNA-seq data.]</figcaption></figure></p>

Indicating that two parametric distributions (examples of parametric distributions could be a *normal distribution* which is identified by its mean and standard deviation; or a *negatively binomial* distribution which is identified by its mean and dispersion) are statistically different from each other is a relatively established process, I have come to understand. However, the scRNA-seq data with its high frequency of zero-drop counts doesn't look like a nice parametric distribution. So new methods of comparitive analysis are required! I wonder what assumptions go in while creating a model based on the real-sequenced data and which tests are predominantly used for non-parametric distributions such as the one in the figure, above.

  