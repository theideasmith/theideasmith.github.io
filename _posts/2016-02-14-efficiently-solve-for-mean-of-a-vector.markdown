---
layout: post
title: Efficiently Solve for Mean of a Vector
date: 2016-02-14T00:00:00-05:00
---

Recently as I was reviewing for the ACTs, of the *low hanging fruit* questions was one that asked to solve for the mean of a set of numbers by hand. Formally, given an n-tuple $x=(x_1,...,x_i,...,x_n)$, I needed to solve for

$$\frac{\sum_{i=0}^n{x_i}}{n}$$

But this method takes more time as the numbers get larger. This question shouldn't take longer than a few seconds so a quicker method would be more efficient. 

I considered and then used this formula:

$$\textbf{x}_{min}+\frac{\sum_{i=0}^n{\textbf{x}_i-\textbf{x}_{min}}}{n}$$

The proof for  $$\textbf{x}_{min}+\frac{\sum_{i=0}^n{\textbf{x}_i-\textbf{x}_{min}}}{n}=\frac{\sum_{i=0}^n{x_i}}{n}$$ is exceedingly simple:

$$\begin{align}
   \textbf{x}_{min}+\frac{\sum_{i=0}^n{\textbf{x}_i-\textbf{x}_{min}}}{n} \tag 1\\
   = \frac{n\textbf{x}_{min}}{n}+\frac{\sum_{i=0}^n{\textbf{x}_i}}{n}-\frac{nx_{min}}{n} \tag 2\\
   = \frac{\sum_{i=0}^n{\textbf{x}_i}}{n}\tag 3\\
\end{align}$$

If you are internally laughing at the triviality of this concept, I concur. Do not make a fundamental attribution error by assuming that my mathematical abilities are limited to this complexity. That I find this worth posting is indicative of the long ways I have to grow and deepen my mathematical understanding. 

My true intent in writing this post was to practice my mathjax skills and to share a quick idea I had. If I don't have time to write about deep ideas, at least I will have shared simpler ones because $1>0$
