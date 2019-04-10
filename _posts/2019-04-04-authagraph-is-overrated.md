---
layout: default
title: Authagraph is Overrated
---
# The AuthaGraph projection is overrated: Here's why
Back in 2016, the AuthaGraph projection took the media by storm when it was awarded Japan's Good Design Grand Award. News outlets claim it to be "the most accurate ever" or any other sensational claims. However, I feel like this projection is severely overrated and all those media have blown this news out of proportion, and I'm here to show you why.
## Its equations have never been published
Mr. Narukawa keeps the equations to make the AuthaGraph projection a trade secret. It's never been published anywhere, and he doesn't need to, because he sees it as a fairly profitable business. With its equations being kept proprietary, applications of this projection in GIS software is impossible, and people who wants a map in this projection must buy it from him.

I don't get why anyone would do this, considering that not even something like the authors of Van der Grinten (in which it used to be patented) or Dymaxion projection (in which the name was trademarked) hide their methods of projection. They all either publish their equations somewhere or show in full detail how to make one. Meanwhile, AuthaGraph only has a really vague explanation on their webpage, which isn't very useful, so people can't really try to make one properly.
## It's not even a new projection
The AuthaGraph projection has been around since 1999, but only managed to gain some attention in 2016, when it was awarded the Japan Good Design Grand Award. This means that even after 20 years of this projection's existence, Mr. Narukawa doesn't want to reveal the equations to create it just yet. Perhaps either when he dies, his company goes bankrupt or someone leaks the equations then we might be able to get it.
## There's a better tetrahedral projection that is conformal and visually more appealing
AuthaGraph isn't the only tetrahedral projection out there, of course. In my opinion, the Lee tetrahedral projection is way better than it. Because it's a conformal projection, the shapes of the continents don't look weird unlike it does in AuthaGraph, since it preserves angles locally.

Not only that, it also maintains area proportions pretty well for a conformal projection. You see, conformal projections are notorious for its terrible areal distortions they usually have, but not with this one, since it's polyhedral and you can configure it so that most, if not all of the continents avoid the regions where distortions are the worst (i.e. the singularities). Any tetrahedral projections can be configured to look like AuthaGraph, including this one, so you can have both the conformality of this projection and the cleverly-done region placements of AuthaGraph at the same time.

<center><a href="https://chemistzombie.files.wordpress.com/2019/04/leetetrahedral-authagraphlike.png"><img src="https://chemistzombie.files.wordpress.com/2019/04/leetetrahedral-authagraphlike.png?w=1024"></a><br />The Lee tetrahedral projection with Authagraph-like configuration.</center>
## The AuthaGraph name is misleading, because it's NOT an equal-area (authalic) projection
AuthaGraph's name was derived from "authalic" (which means equal-area) and "-graph". However, an analysis of a [reverse-engineered version](https://kunimune.home.blog/2017/11/23/the-secrets-of-the-authagraph-revealed/) of this projection shows that it's not equal-area, but rather a compromise projection. Equal-area tetrahedral projections do exist, such as the [van Leeuwen projection](https://doi.org/10.1559/152304006779500687), but not this one.