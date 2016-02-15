# Overview

The World Map presents the player important data regarding the game. It contains several elements like fixed or mobile servers, missions, buildings and general points of interest.

It is notably the main way a player has to interact with the virtual world that surrounds him. It also has become the most important aspect of the game.

# Distribution

By default, we implement a global grid made of squares with size equal 0.005 latitude(φ)/longitude(λ). However, the Earth is not a perfect sphere, it actually has an irregular shape, making this problem extremely complex.

Having a grid with height of `0.005°` latitude, width of `0.005°` longitude eases the complex operations we have to do over that data, but we need to keep in mind we have different-sized squares over the planet. For example, squares around equator would be much smaller than squares near the poles.

That said, we'll apply a dynamic density distribution over the game, with the intent of better handling highly crowded areas. The algorithm will shrink, or expand those grid squares according to how many players we have in that specific region.

# Influence

Influence is the defining factor of power, or respect, of the game. It tells how powerful a hacker *currently* is. 

Any remote action taken by the hacker is translated into influence. The attacker gains influence where his access-point (origin) is located, as well as where his gateway (target) is.

## Spread

The spread of influence is analogous to sand falling to the floor and forming a pile. When an action that deserves influence is completed, a relative amount of influence will "fall" into the origin and target of the action. As it falls, influence is spread to all sides, being greater on the center, and slowly fading away as it goes further.

The spread speed is defined in turns of one hour. The next turn right after the attack is turn 1, where the grid square of the attack ("center") receives 100% of the relative influence. On the next turn, the neighbors squares receive a smaller percent, and so on.

Influence also accumulates on the center, creating a notion of z-axis influence.

[TODO: Spread is actually much more complex than this. Explain better.]

