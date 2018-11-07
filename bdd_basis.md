---
layout: post
title: BDD Basis
landing-title: 'BDD Basis'
nav-menu: true
description: null
image: null
author: null
---

A Boolean function can be represented as a rooted, directed, acyclic graph, which consists of several decision nodes and terminal nodes. There are two types of terminal nodes called 0-terminal and 1-terminal. Each decision node {\displaystyle N} N is labeled by Boolean variable {\displaystyle V_{N}} V_N and has two child nodes called low child and high child. The edge from node {\displaystyle V_{N}} V_N to a low (or high) child represents an assignment of {\displaystyle V_{N}} V_N to 0 (resp. 1). Such a BDD is called 'ordered' if different variables appear in the same order on all paths from the root. A BDD is said to be 'reduced' if the following two rules have been applied to its graph:
Merge any isomorphic subgraphs.
Eliminate any node whose two children are isomorphic.
In popular usage, the term BDD almost always refers to Reduced Ordered Binary Decision Diagram (ROBDD in the literature, used when the ordering and reduction aspects need to be emphasized). The advantage of an ROBDD is that it is canonical (unique) for a particular function and variable order.[1] This property makes it useful in functional equivalence checking and other operations like functional technology mapping.
A path from the root node to the 1-terminal represents a (possibly partial) variable assignment for which the represented Boolean function is true. As the path descends to a low (or high) child from a node, then that node's variable is assigned to 0 (resp. 1).
