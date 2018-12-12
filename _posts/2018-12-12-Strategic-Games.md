---
layout: post
title: Strategic Games
---

## Definitions
A strategic games is a model of interactive decision-making in which each decision-maker selects his plan of action once and for all, and these choices are made simultaneously. The formal definition of a strategic game is shown as following.

* A strategic game consists of
  + a finite set $N$ (the set of **players**)
  + for each player $i \in N$ a nonempty set $A_{i}$ (the set of **actions** available to player $i$)
  + for each player $i \in N$ a preference relation $\succsim_{i}$ on $A = \times_{j \in N} A_{j}$ (the **preference relation** of player $i$).

If the set $A_{i}$ of actions of every player $i$ is finite then the game is *finite*. We refer to an action profile  as an outcome, and denote the set $\times_{j \in N} A_{j}$ of outcomes by $A$. Therefore, each player may care not only about his own action but also about the actions taken by the other players, which is the feature that distinguishes a *strategic game* from a *decision problem*.

Under a wide range of circumstances the preference relation $\succsim_{i}$ of player $i$ in a strategic game can be represented by a **payoff function** $u_{i}: A \rightarrow \mathbb{R}$ (also called a *utility function*), in the sense that $u_{i}(a) \geq u_{i}(b)$ whenever $a \succsim_{i} b$. We refer to values of such a function as **payoffs** (or utilities). Thus, we usually denote the game by $\langle N, (A_{i}), (u_{i}) \rangle$ rather than $\langle N, (A_{i}), (\succsim_{i}) \rangle$.
