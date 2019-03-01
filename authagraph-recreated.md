---
layout: default
title: The AuthaGraph projection has been recreated fairly successfully (with images)
---
# Authagraph, recreated
The AuthaGraph projection is a compromise tetraheadral projection that won Japan's Good Design Grand Award in 2016. There's actually nothing special to this projection, really. It's simply a compromise projection that tries to minimize land distortions, dumping most of them into the oceans (which in turn makes it unsuitable for ocean-related thematic maps). However, news outlets have literally exaggerated this, claiming that it's "[the most accurate projection ever](https://www.thesun.co.uk/news/2108192/japanese-origami-authagraph-map-hailed-the-most-accurate-ever-made-unfolds-the-globe-so-countries-appear-the-right-size/)" or something similar, when in fact it's nothing other projections can't do, like Winkel tripel or Robinson projections (that's why you shouldn't believe the hype and marketing).

If for some reason you want to use this projection, unfortunately you can't. That's because Narukawa (creator of this projection) hasn't published its equations, and I highly doubt he'd be willing to do so, considering that he turned it into a fairly profitable business, even going as far as to make a company under the same name.

However, some people have attempted to recreate this projection, particularly [Marcin Ciura](https://marcinciura.wordpress.com/2016/11/20/authagraph/), [Justin Kunimune](https://kunimune.home.blog/2017/11/23/the-secrets-of-the-authagraph-revealed/), and [Tobias Jung](https://blog.map-projections.net/an-equal-area-projection-in-the-fashion-of-the-authagraph-map). But so far the best one is Kunimune's recreation, which looks so similar to the original one you might not be able to notice the difference without comparison figures.

Additionally, the equations for this AuthaGraph clone, along with his map projection tool, is publicly available on [GitHub](https://github.com/jkunimune15/Map-Projections)

# Images
Here are some images to enjoy (as well as to annoy Narukawa for not publishing his equations XD). Highest resolution images are 9459x4096 pixels large, but some have lower resolutions due to long render times when outputting these maps at high resolution.

![](/images/kunimunes-authagraph-4096p.jpg)
*The projection applied on the Blue Marble Earth map (which is included in the tool). Note that Narukawa hasn't published surface maps like this with his AuthaGraph projection*

![](/images/kunimunes-authagraph-4096p-incl-polar-icecaps.jpg)
*Alternative version. Original (10K) image [here](http://planetpixelemporium.com/earth8081.html)*

![](/images/authaoverlay.png)
*Overlay map that shows the map's distortions. Red areas are compressed, blue areas are dilated, and black areas are stretched. You can notice that the most severe distortions are confined to the oceans and Siberia (which is one of this projection's weaknesses, so much for being "the most accurate")*

![](/images/authagraph-tissot.png)
*The AuthaGraph clone projection with Tissot indicatrices every 15 degrees.*