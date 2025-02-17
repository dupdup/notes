---
layout: default
title: Algorithms
description: Notes on algorithms.
nav_order: 2
has_children: true
has_toc: false
parent: Data structures and algorithms
permalink: /data-structures-and-algorithms/algorithms
---

<!-- prettier-ignore-start -->

# Algorithms
{:.no_toc}

## Table of contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Introduction

An algorithm is a procedure that takes input and produces output that accomplishes a specific task {% cite algorithm-design-manual -l 3 %}.

An algorithm should solve a general, well-specified problem. A specification for an algorithm should include the complete set of instances it will operate on, and the algorithm's output after running on one of these instances {% cite algorithm-design-manual -l 3 %}.

A good algorithm is:

- Correct
- Efficient
- Easy to implement

It's not always possible to meet these goals {% cite algorithm-design-manual -l 4 %}.

An algorithm is commonly expressed in one of the following forms:

1. English
2. Pseudocode
3. A programming language

{% cite algorithm-design-manual -l 12 %}

## Reasoning about correctness

The most important property of an algorithm is that it's correct.

One way to demonstrate the correctness of an algorithm is a mathematical proof.

A mathematical proof consists of four parts:

1. A statement of what you're trying to achieve
2. A set of assumptions you take to be true
3. A chain of reasoning that takes you from the assumptions to the statement you are attempting to prove
4. A little square (∎) or QED to denote the end of the proof

{% cite algorithm-design-manual -l 11 %}

### Problems and properties

In order to demonstrate correctness, your problem must be well-specified.

Problem specifications have two parts:

1. The set of allowed input instances
2. The required properties of the algorithm output

{% cite algorithm-design-manual -l 12 %}

You should avoid asking ill-defined questions. Asking "what is the best path?" is ill-defined: what does _best_ mean? You should be more specific, for example: "which is the _fastest_ path to take?" {% cite algorithm-design-manual -l 13 %}.

### Demonstrating incorrectness

You can prove an algorithm incorrect by providing an input that produces the incorrect output. These are called **counter-examples** {% cite algorithm-design-manual -l 13 %}.

Good counter-examples are verifiable and simple {% cite algorithm-design-manual -l 13 %}.

### Induction and recursion

Failure to prove an algorithm as incorrect does not make it correct. **Mathematical induction** is a common method to prove the correctness of an algorithm.

The way to prove a predicate (P) through induction is to:

- Prove the case P(0)
- Assume that P(k) is true
- Prove P(k+1)

_see this [video teaching proof by induction](https://www.youtube.com/watch?v=wblW_M_HVQ8) for further explanation_

### Sigma notation

Summations are common in algorithm analysis.

Sigma notation is a way of expressing summation formulas. For example, the sum of 1 to n in sigma notation is:

$$\sum_{i=1}^{n} i$$

_see this [video explaining sigma notation](https://www.youtube.com/watch?v=5jwXThH6fg4) for further explanation_

## Modelling the problem

Modelling is the process of formulating your application in terms of well-defined, well-understood problems. Modelling can eliminate the need to create your own algorithm, since you can rephrase your problem to use a pre-written algorithm {% cite algorithm-design-manual -l 19 %}.

Most problems are real-world problems. For example, you might need to create a system to route traffic. Algorithms don't work on real-world objects, they work abstractions, like a graph. In order to write effective algorithms you must learn how to describe your problems in terms of abstract strictures {% cite algorithm-design-manual -l 19 %}.

In order to model a problem, you should have a solid understanding of the [data structures](../data-structures-and-algorithms/data-structures.md) available to you.

## Conclusion

Algorithms are procedures that accomplish a specific task.

You can determine the correctness of an algorithm using a mathematical proof, one way of doing this is by using mathematical induction.

Algorithms work on abstract objects. In order to write algorithms for real-world problems, you need to model your real-world problems in terms of abstract objects that an algorithm can work on.

## References

{% bibliography --cited_in_order %}
