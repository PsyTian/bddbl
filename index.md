---
layout: home
title: Home
landing-title: 'BDDBL Denotes Dummy BDD Library'
description: null
image: null
author: null
---

Binary Decision Diagram (BDD) is a family of data structure used to represent Boolean functions[3]. Reduced Ordered Binary Decision Diagram (ROBDD) is the most common form of BDD in applications in computer science. ROBDDs keeps variables canonical and ordered. These properties offer convenience for functional equivalence checking, functional mapping, etc. A BDD is constructed by three types of nodes: root nodes, branch nodes and sink nodes. Every root node or branch node can be represent with a world with three fields, <V,LO,HI>, where V represents the index of the variable, LO represents the successors when the value of the variable is 0 (or False), and HI represents the Ture one. The value LO and HI can either be a pointer of the successor or a value representing False and True, which means the succeeding node is a sink node. There are many BDD packages for manipulating BDDs and variants, with Dynamic variable reordering , breadth-first manipulating built in. CUDD, BuDDy and JavaBDD are most widely used packages, and PPBF tried to develop a parallel implementation.
