---
layout: post
title: Strictly Competitive Games
---

In short words, strictly competitive games are a special type of strategic games whose preferences are completely opposed. The formal definition is shown as following.

* A strategic game $\langle \{1,2\}, (A_{i}), (\succsim_{i}) \rangle$ is **strictly competitive** if for any $a \in A$ and $b \in A$ we have $a \succsim_{1} b$ if and only if $b \succsim_{2} a$.

A strictly competitive game is sometimes called *zero-sum* because if player 1's preference relation $\succsim_{1}$ is represented by the payoff function $u_{1}$ then player 2's preference relation is represented by $u_{2}$ with $u_{1} + u_{2} = 0$.

Literally, the procedure of the strictly competitive games can be explained that player *i* *maxminimizes* if he chooses an action that is best for him on the assumption that whatever he does, player *j* will choose her action to hurt him as much as possible. The formal definition of a strictly competitive game is shown as following.

* Let $\langle \{1,2\}, (A_{i}), (\succsim_{i}) \rangle$ be a strictly competitive strategic game. The action $x^{*} \in A_{1}$ is a **maxminimizer** for player 1 if

$$\min_{y \in A_{2}} u_{1}(x^{*}, y) \geq \min_{y \in A_{2}} u_{1}(x, y) \text{ for all } x \in A_{1}.$$

Similarly, the action $y^{*} \in A_{2}$ is a **maxminimizer** for player 2 if

$$\min_{x \in A_{1}} u_{2}(x, y^{*}) \geq \min_{x \in A_{1}} u_{2}(x, y) \text{ for all } y \in A_{2}.$$

In words, a maxminimizer for player *i* is an action that maximizes the payoff that player *i* can *guarantee*. There are some important properties of strictly competitive games shown as following.

* Let $G = \langle \{1,2\}, (A_{i}), (u_{i}) \rangle$ be a strictly competitive strategic game.
    + If $(x^{\*}, y^{\*})$ is a Nash equilibrium of G then $x^{\*}$ is a **maxminimizer** for player 1 and $y^{\*}$ is a **maxminimizer** for player 2.
    + If $(x^{\*}, y^{\*})$ is a Nash equilibrium of *G* then $\max_{x} \min_{y} u_{1}(x, y) = \min_{y} \max_{x} u_{1}(x, y) = u_{1}(x^{\*}, y^{\*})$, and thus all Nash equilibria of *G* yield the same payoffs.
    + If $\max_{x} \min_{y} u_{1}(x, y) = \min_{y} \max_{x} u_{1}(x, y)$, $x^{\*}$ is a **maxminimizer** for player 1, and $y^{\*}$ is a **maxminimizer** for player 2, then $(x^{\*}, y^{\*})$ is a Nash equilibrium of *G*.

By the third statement above, we can find the players' Nash equilibrium strategies by solving the problems $\max_{x} \min_{y} u_{1}(x, y)$ and $\max_{y} \min_{x} u_{2}(x, y)$. Because of the first and the third statements above, we can conclude that the Nash equilibria of a strictly competitive game are **interchangeable**: if $(x, y)$ and $(x', y')$ are equilibria then so are $(x, y')$ and $(x', y)$. If $\max_{x} \min_{y} u_{1}(x, y) = \min_{y} \max_{x} u_{1}(x, y)$ then we say that this payoff, the equilibrium payoff of player 1, is the **value** of the game.
