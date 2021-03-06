---
layout: post
title: A Brief Overview on Game Theory
---

## What is Game Theory?
Game theory is a subject that helps us to realize the phenomena caused by the interaction of decision-makers. The fundamental assumption of game theory is that every decision-maker persues an exogenous objective while considers other decision-makers' behaviours. Actually, game theory does nothing but constructs some abstract models that can reflect the real-life situations. 

## Games and Solutions
In general, the template of game theory involves two parts, a game and a solution. Specifically, a game is a description of strategic interaction that includes the actions that the players interests or the players can conduct, but excluding the actions that the players actually take. A solution is a systematic description of the outcomes that may emerge in a family of games, and this solution should be reasonable.

### Non-cooperative and Cooperative Games
In game theory, a player can be regarded as an individual or a group of decision-makers. Those in which the sets of possible actions of individual players are primitives are referred to as non-cooperative whereas those in which the sets of possible joint actions of groups of players are primitives are referred to as cooperative.

### Strategic Games and Extensive Games
A strategic game is a model of a situation in which each player selects his plan of actions once and all of players' decisions are made simultaneously. During the procedure, no player is informed of the plan of actions chosen by other players. By contrast, the model of an extensive game specifies the possible sequences of events where each player can take into account of his plan of action not only at the beginning of the game but also the intermediate stage.

### Games with Perfect and Imperfect Information
A game with perfect information means that all of participants are fully informed of the other players' actions, while a game with imperfect information indicates players are not perfectly informed.

## Rational Behavior
In game theory, the models we study assume that each decision-maker is rational in the sense that he is aware of his alternatives, forms expectations about any unknowns, has clear preferences, and chooses his action deliberately after some process of optimization. 

In the absence of uncertainty the following elements constitute a model of rational choice:
- A set $A$ of actions from which the decision-maker makes a choice.
- A set $C$ of possible consequences of these actions.
- A consequence function $g: A \rightarrow C$ that associates a consequence with each action.
- A preference relation $\succsim$ on the set $C$.

Sometimes the decision-maker's preferences are specified by giving a utility function $U: C \rightarrow \mathbb{R}$, which defines a preference relation $\succsim$ by the condition $x \succsim y$ if and only if $U(x) \geq U(y)$.

Given any set $B \subseteq A$ of actions that are feaible in some particular case, a rational decision-maker selects an action $a^{\*}$ that is feasible (belongs to $B$) and optimal in the sense that $g(a^{\*}) \succsim g(a)$ for all $a \in B$; alternatively he solves the problem $\max_{a \in B} U(g(a))$.

## The Steady State and Deductive Interpretations
There are two conflicting interpretations of solutions for strategic and extensive games, the steady state interpretation and the deductive interpretation. The steady state interpretation treats a game as a model designed to explain some regularity observed in a family of similar solutions. Each participant knows the equilibrium and tests the optimality of his behavior given this knowledge, which he has acquired from his long experience. The deductive interpretation, by contrast, treats a game in isolation, as a one-shot event, and attempts to infer the restrictions that rationality imposes on the outcome. It assumes that each player deduces how the other players will behave simply from principles of rationality.

## Bounded Rationality
When we talk in real life about games we often focus on the asymmetry between individuals in their abilities. These differences, which are so critical in life, are missing from game theory in its current form. Modelling asymmetries in abilities and in perceptions of a situation by different players is a fascinating challenge for future research, which models bounded rationality have begun to tackle.
