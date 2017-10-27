---
layout: post
title: Solving the Game of Set with Machine Vision
description: Machine Vision Project
img: /img/set.jpg
---

In this project, I worked on a solver for the <a href="https://en.wikipedia.org/wiki/Set_%28game%29" target="blank">game of set</a>.

Set is a game in which 12 cards are laid out in front of several players. Each card posses one of 3 variations for 4 distinct features : number (one, two or three), shape (oval, diamond or squiggle), color (purple, green and red) and shading (full, empty, shaded).

Players try to find a set of 3 cards in which the features are either all the same or all different.



<div class="img_row">
	<img class="col three" src="{{ site.baseurl }}/img/set.jpg" alt="" title="game of set"/>
</div>
<div class="col three caption">
	An example of a typical game of set.
</div>

In this game the solution is hidden in plain sight. It can often take minutes to solve a problem. I developed a Machine Vision program using openCV to detect the sets hidden in the image.

The Program detects all 4 features within each card and uses the data to find sets in the image.



<br/><br/><br/>


