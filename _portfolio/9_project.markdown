---
layout: post
title: Expert System for Machining
description: AI for Tooling
img: /img/part.jpg
---

The purpose of this project was to program an artificial intelligence capable of choosing best tools and operations to machine a part.

For this project, I used <a href="https://en.wikipedia.org/wiki/CLIPS" target="blank">Clips</a>, an open source software developed by NASA to build <a href="https://en.wikipedia.org/wiki/Expert_system" target="blank">expert systems</a>. 

This type of system is programmed by defining rules to replicate the reasoning of an expert in machining.

First, I defined:
 
* the part I wanted to machine by describing it with a list of features (for example, feature 1: through hole, diameter : 12mm, direction x-axis). 
* the capability of the machines available in my shop (example for a 3 axis milling machine I would define the machine as: Milling machine, directions available x-axis, y-axis z-axis) 
* And the tools available (for example, type: drill bit, diameter : 12mm, length 100 mm)

I used my knowledge in machining to define a set of rule. For example:

	The hole can be made with drill bit A
	if the diameter is of A is equal to the diameter of the hole
	and if the length of A is greater than the depth of the hole

Running the program lead for each feature, to the choice of:
* The Tools
* The Machine to be used 
* The Machining Direction


The last step was to define the order of the operations to make the part based on another set of rules


<div class="img_row">
	<img class="col two" src="{{ site.baseurl }}/img/part.jpg" alt="" title="part to make"/>
	<img class="col one" src="{{ site.baseurl }}/img/clips.jpg" alt="" title="clips project"/>
</div>
