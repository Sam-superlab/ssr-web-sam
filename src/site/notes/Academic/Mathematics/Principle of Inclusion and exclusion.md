---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Principle of Inclusion and exclusion/"}
---

We suppose there is a list of property and we assume there is a certain subset of elements that have the property and the rest of the elements do not. We want to get the number of elements that have none of the properties:

- Let $N_{0}=n$
- Count the number of objects having each property which is $\binom{n}{1}$, and let $N_{1}$ be the result
- In general look at the $\binom{k}{i}$ possible subsets of $i$ properties. For each of these we count the number of objects haaving all $i$ properties in the subset. THen add up all these numbers call it $N_i$

>Theorem: Suppose given k properties and given an n-set X let $N_{0} , ... , N_{k}$ be as defined above. Then the number M of elements with none of the properties is given by the formula:
>$$M = \sum_{i=0}^{k} (-1)^{i} N_{i}$$


