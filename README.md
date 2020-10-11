# Overview of the Problem:

In this model, we are going to consider **edit distance** between every pair of words in a list containing the vocabulary. Basically, edit distance is a **measure of minimum edits required to convert one word to another**.  
This process of conversion includes steps like **Delete**,**Replace**,**Switch** and **Insert** on a pair of words. In this blog, to reduce complexity, we would go for words that are **1 or 2 edit distance away**.  
The goal of our model to produce the right output is to compute the **probability of a word being correct, _P(c/w)_ ,is probability of certain word _w_ given that is is correct, _P(w/c)_ , multiplied to probability of being correct in general, _P(c)_ , divided by probability of that word appearing, _P(w)_ .**

Formula : **𝑃(𝑐|𝑤)=𝑃(𝑤|𝑐)×𝑃(𝑐)/𝑃(𝑤)**

The method used above is called **Bayes Theorem**.