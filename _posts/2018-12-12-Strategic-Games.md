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

If the set $A_{i}$ of actions of every player $i$ is finite then the game is *finite*. We refer to an action profile $a = (a_{j})$ as an outcome, and denote the set $\times_{j \in N} A_{j}$ of outcomes by $A$. Therefore, each player may care not only about his own action but also about the actions taken by the other players, which is the feature that distinguishes a *strategic game* from a *decision problem*.

Under a wide range of circumstances the preference relation $\succsim_{i}$ of player $i$ in a strategic game can be represented by a **payoff function** $u_{i}: A \rightarrow \mathbb{R}$ (also called a *utility function*), in the sense that $u_{i}(a) \geq u_{i}(b)$ whenever $a \succsim_{i} b$. We refer to values of such a function as **payoffs** (or utilities). Thus, we usually denote the game by $\langle N, (A_{i}), (u_{i}) \rangle$ rather than $\langle N, (A_{i}), (\succsim_{i}) \rangle$.

For example, in the table below it shows a representation of a strategic game. The set of actions of the row player is $\{ T, B \}$ and that of the column player is $\{ L, R \}$. For instance, the row player's payoff from the outcome $(T, L)$ is $w_{1}$ and the column player's payoff is $w_{2}$. In convention, we name the row player as player 1 and the column player as player 2.

|     |      **L**     |      **R**     |
|:-----:|:----------------:|:----------------:|
|**T**| $\ \ \tiny w_{1}, w_{2}$ | $\ \ \tiny x_{1}, x_{2}$ |
|**B**| $\ \ \tiny y_{1}, y_{2}$ | $\ \ \tiny z_{1}, z_{2}$ |

## Intepretation
A common interpretation of a strategic game is that it is a model of an event that occurs only once. Each player knows the details of the game and the fact that all the players are rational, and the players select their actions simultaneously and independently.

Another interpretation is that a player can form his expectation of the other players' behaviour on the basis of information about the way that the game or a similar game was played in the past.

When referring to the actions of the players in a strategic game as simultaneous we do not necessarily mean that these actions are taken at the same point in time. For the situation to be modeled as a strategic game it is important only that the players make decisions independently, no player being informed of the choice of any other player prior to making his own decision.

## Nash Equilibrium
Nash Equilibrium is the most commonly used solution concept in game theory. This notion captures a *steady state* of the play of a strategic game in which each player holds the correct expectation about the other players' behavior and acts rationally. The complete definition of Nash equilibrium is shown as following.

Definitions A Nash equilibrium of a strategic game $\langle N, (A_{i}), (\succsim_{i}) \rangle$ is a profile $a^{*} \in A$ of actions with the property that for every player $i \in N$ we have

$$(a^{*}_{-i}, a^{*}_{i}) \succsim_{i} (a^{*}_{-i}, a_{i}) \text{ for all } a_{i} \in A_{i}.$$

In English, Nash equilibrium means no player can profitably deviate, given the actions of the other players. Besides, we can use another statement to describe Nash equilibrium. For any $a_{-i} \in A_{-i}$ define $B_{i}(a_{-i})$ to be the set of player *i*'s best actions given $a_{-i}$:

$$B_{i}(a_{-i}) = \{ a_{i} \in A_{i}: (a_{-i}, a_{i}) \succsim_{i} (a_{-i}, a_{i}’) \text{ for all } a_{i}{'} \in A_{i} \}.$$

We call  the set-valued function $B_{i}$ the **best-response function** of the player *i*. A Nash equilibrium is a profile $a^{*}$ of actions for which

$$a_{i}^{*} \in B_{i}(a_{-i}^{*}) \text{ for all } i \in N.$$

## Existence of a Nash Equilibrium
An existence result has two purposes. First, if we have a game that satisfies the hypothesis of the result then we know that there is some hope that our efforts to find an equilibrium will meet with success. Second, and more important, the existence of an equilibrium shows that the game is consistent with a steady state solution. The formal proposition to show the existence of Nash equilibrium in a strategic game is stated as following.

* The strategic game $\langle N, (A_{i}), (\succsim_{i}) \rangle$ has a Nash equilibrium if for all $i \in N$
  + the set $A_{i}$ of actions of player $i$ is a nonempty compact convex subset of a Euclidian space
  + the preference relation $\succsim_{i}$ is
    - continuous
    - quasi-concave on $A_{i}$

Note that the proposition above does not apply to any game in which some player has finitely many actions, since such a game violates the condition that the set of actions of every player be convex.
