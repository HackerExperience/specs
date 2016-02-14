# World Map

## Overview

The World Map presents the player important data regarding the game. It contains several elements like fixed or mobile servers, missions, buildings and general points of interest.

It is notably the main way a player has to interact with the virtual world that surrounds him.

## Distribution

By default, we implement a global grid made of squares with size equal 0.005 latitude(φ)/longitude(λ). However, the Earth is not a perfect sphere, it actually has an irregular shape, making this problem extremely complex.

Having a grid with height of `0.005°` latitude, width of `0.005°` longitude eases the complex operations we have to do over that data, but we need to keep in mind we have different-sized squares over the planet. For example, squares around equator would be much smaller than squares near the poles.

That said, we'll apply a dynamic density distribution over the game, with the intent of better handling highly crowded areas. The algorithm will shrink, or expand those grid squares according to how many players we have in that specific region.

