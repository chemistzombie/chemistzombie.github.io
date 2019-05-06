# New pseudoazimuthal projections
It turns out it's actually quite easy to make pseudoazimuthal projections without the knowledge of making the equations for it. They are made by halving the longitudes, projecting it to an azimuthal projection, and stretching the result into a 2:1 ellipse. Using an image editor and map projection software, one can do the following to get the same results:

1. Using an image editor, compress an equirectangular world map into a 1:1 square, and then edit the canvas size so that the width is twice the height of it again. This is done to avoid the projection software from correcting the map's aspect ratio.
2. Project the equirectangular map with an azimuthal projection and limit the projection range to a hemisphere. This is not possible with gnomonic or vertical perspective projections, meaning that they won't show the entire world.
3. Stretch the result so the width becomes twice the height of the image again, and you're done.

The only drawbacks of using this method are you won't get to know the equations, everything has to be done manually, and you can't get a visualization for the distortion patterns of the projections.

## Airy pseudoazimuthal
The Airy projection is a minimum-error azimuthal projection designed to minimize areal and angular distortions.

Quoting from Snyder's "Flattening the Earth" book:

> [Airy] approached the development of his projection with a goal of having a minimum "total evil" determined by what he called "Balance of Errors". His "Projection by Balance of Errors" is neither perspective, conformal, nor equal-area, but it is a compromise appearing very much like the azimuthal equidistant projection, especially if limited to about one hemisphere.
> Airy's specific approach was to minimize the sum of the squares of the erors in scale both along and perpendicular to the radii from the center of projection. For the polar aspect, these measurements are along meridians and parallels, respectively.

I'm not really sure if the pseudoazimuthal version is also good enough in minimizing distortions, but it's definitely a compromise projection.

<center><a href="https://3.bp.blogspot.com/-xWiW6YF3izk/XNCAPamJsxI/AAAAAAAAAZI/WZV8ER_m8akMA9JLgyLPo2w90-gzrMs2ACLcBGAs/s0/airy_pseudoazimuthal.png"><img src="https://3.bp.blogspot.com/-xWiW6YF3izk/XNCAPamJsxI/AAAAAAAAAZI/WZV8ER_m8akMA9JLgyLPo2w90-gzrMs2ACLcBGAs/s640/airy_pseudoazimuthal.png"></a></center>
## Breusing geometric pseudoazimuthal
The Breusing geometric projection is another minimum-error azimuthal projection. It balances the shape distortion of the azimuthal equal-area projection and the area distortion of the conformal stereographic projection by using for a given point a radius from the projection center equal to the geometric mean of the radii as calculated for these two projections.

<center><a href="https://4.bp.blogspot.com/-Tr_o6HAffe8/XNCDLnP3GBI/AAAAAAAAAZw/Rs0hO06U4BsCWmFBdPdQRn90iGpOCBcPACLcBGAs/s0/breusing-geometric_pseudoazimuthal.png"><img src="https://4.bp.blogspot.com/-Tr_o6HAffe8/XNCDLnP3GBI/AAAAAAAAAZw/Rs0hO06U4BsCWmFBdPdQRn90iGpOCBcPACLcBGAs/s640/breusing-geometric_pseudoazimuthal.png"></a></center>
## Breusing harmonic pseudoazimuthal
The Breusing harmonic projection is a modification of the Breusing geometric, named so because it uses the harmonic mean of the same base projections as those used by Breusing for his geometric mean, namely, the stereographic and the Lambert azimuthal equal-area projections. In appearance, it strongly resembles the Airy projection.

<center><a href="https://4.bp.blogspot.com/-r8H0oPB0xtE/XNCEAP7boXI/AAAAAAAAAZ4/A-hDSwnPmQkSGIlE1Un2aW9TOBmywaQ9wCLcBGAs/s0/breusing-harmonic_pseudoazimuthal.png"><img src="https://4.bp.blogspot.com/-r8H0oPB0xtE/XNCEAP7boXI/AAAAAAAAAZ4/A-hDSwnPmQkSGIlE1Un2aW9TOBmywaQ9wCLcBGAs/s640/breusing-harmonic_pseudoazimuthal.png"></a></center>
## Gott-Mugnolo pseudoazimuthal
The Gott-Mugnolo azimuthal projection was designed to [minimize distance errors](https://www.utpjournals.press/doi/abs/10.3138/carto.42.3.219). It is based on the azimuthal equal area projection, so the end result looks rather similar to the Hammer projection, but is a compromise projection. 

<center><a href="https://1.bp.blogspot.com/-lTd2YXIOl_0/XNCEcIUwYOI/AAAAAAAAAaE/_Q8ORtP1ZmIZQEj6iN2pIesWsnBQjTLEgCLcBGAs/s640/gott-mugnolo_pseudoazimuthal.png"><img src="https://1.bp.blogspot.com/-lTd2YXIOl_0/XNCEcIUwYOI/AAAAAAAAAaE/_Q8ORtP1ZmIZQEj6iN2pIesWsnBQjTLEgCLcBGAs/s0/gott-mugnolo_pseudoazimuthal.png"></a></center>
## Pseudognomonic
The gnomonic projection can only show less than a hemisphere, and forcing it to go very close to it will cause severe distortions. It's still possible to create a local or regional map with this though.

<center><a href="https://1.bp.blogspot.com/-Jy7xCYS-JuM/XNCFg2TzKtI/AAAAAAAAAac/a7cLGE5d4Scl2Pp7HYWtJUkUqofzU06rACLcBGAs/s0/gnomonic_0.25_pseudoazimuthal.png"><img src="https://1.bp.blogspot.com/-Jy7xCYS-JuM/XNCFg2TzKtI/AAAAAAAAAac/a7cLGE5d4Scl2Pp7HYWtJUkUqofzU06rACLcBGAs/s640/gnomonic_0.25_pseudoazimuthal.png"></a><br />The pseudognomonic projection showing a half of the world. Distortions are still acceptable at this scale.</center>

<center><a href="https://2.bp.blogspot.com/-EvXHW5ZPd3k/XNCGA2W5WfI/AAAAAAAAAaw/pxHxaq-NpUsSNSQ8jfRU2yI2kCWprasbwCLcBGAs/s0/gnomonic_1-3_pseudoazimuthal.png"><img src="https://2.bp.blogspot.com/-EvXHW5ZPd3k/XNCGA2W5WfI/AAAAAAAAAaw/pxHxaq-NpUsSNSQ8jfRU2yI2kCWprasbwCLcBGAs/s640/gnomonic_1-3_pseudoazimuthal.png"></a><br />The pseudognomonic projection showing two-thirds of the world. Distortions have started to become noticeable at this scale.</center>

<center><a href="https://3.bp.blogspot.com/-bdSLuoZG5p8/XNCGccsnLiI/AAAAAAAAAa4/rZWI4k81F8U7w0Jf0LLevopUCRbz6IAawCLcBGAs/s0/gnomonic_85deg_pseudoazimuthal.png"><img src="https://3.bp.blogspot.com/-bdSLuoZG5p8/XNCGccsnLiI/AAAAAAAAAa4/rZWI4k81F8U7w0Jf0LLevopUCRbz6IAawCLcBGAs/s640/gnomonic_85deg_pseudoazimuthal.png"></a><br />The pseudognomonic projection showing 17/18th (around 94.4%) of the world. Distortions are so extreme the map is practically useless and ridiculous.</center>

## Pseudorthographic
This was developed by Daniel Strebe (developer of Geocart) [in 2016](https://www.mapthematics.com/ProjectionsList.php?Projection=298#pseudorthographic), so you might find the equations there. I made this thing manually though since Geocart is expensive as hell.

It's able to show the entire world because an orthographic projection projects the earth from an infinite distance, which means it's able to show a whole hemisphere, which is exactly what's needed to create the pseudoazimuthal projection.

The projection looks pretty awful though, so I don't see any reasons for anyone to use this. Landmasses near the center of the map are significantly inflated, while those on the edge of the map are shrunk down and barely noticeable. It also loses the common purpose of having an orthographic map in the first place: to simulate a globe.

<center><a href="https://2.bp.blogspot.com/-1pLvFnc9k1s/XNCFLhpnm4I/AAAAAAAAAaU/8Nowhq-ha98GQcq8hUesTUoG00wPOTU4ACLcBGAs/s0/pseudoorthographic.png"><img src="https://2.bp.blogspot.com/-1pLvFnc9k1s/XNCFLhpnm4I/AAAAAAAAAaU/8Nowhq-ha98GQcq8hUesTUoG00wPOTU4ACLcBGAs/s640/pseudoorthographic.png"></a></center>

## Pseudostereographic
This was developed by Justin Kunimune in 2017 and is available in his [Map Designer](https://github.com/jkunimune15/Map-Projections) software. He described it as "the next logical step after Aitoff and Hammer". Despite being based on the stereographic projection, which is conformal, the resulting map isn't. However, the angular deformations are somewhat more controlled here at the cost of having a much higher areal distortion than Aitoff or Hammer.

Because this projection exists in the Map Analyzer/Designer software he made, the distortion patterns can be visualized with it.

<center><a href="https://2.bp.blogspot.com/-YJQhhYme-TY/XNCHP2-sFxI/AAAAAAAAAbM/A6M2rdDKsIAFp1lAUxPpcOt9wi-yX8DHQCLcBGAs/s0/pseudostereographic.png"><img src="https://2.bp.blogspot.com/-YJQhhYme-TY/XNCHP2-sFxI/AAAAAAAAAbM/A6M2rdDKsIAFp1lAUxPpcOt9wi-yX8DHQCLcBGAs/s640/pseudostereographic.png"></a><br />This one was made using Map Designer instead of by hand.</center>

<center><a href="https://3.bp.blogspot.com/-UJL-htQzbuI/XNCHQWZiUGI/AAAAAAAAAbE/K06DShTXINcPpXbsr10kKBKZojF-fdSgwCLcBGAs/s0/pseudostereographic_distortions.png"><img src="https://3.bp.blogspot.com/-UJL-htQzbuI/XNCHQWZiUGI/AAAAAAAAAbE/K06DShTXINcPpXbsr10kKBKZojF-fdSgwCLcBGAs/s320/pseudostereographic_distortions.png"></a><a href="https://1.bp.blogspot.com/-e4dD15Ut_ig/XNCHQiRC4CI/AAAAAAAAAbI/uuLJZgOsYQAlN9YjES4RGgmRF8_-cL6qACLcBGAs/s0/aitoff_distortions.png"><img src="https://1.bp.blogspot.com/-e4dD15Ut_ig/XNCHQiRC4CI/AAAAAAAAAbI/uuLJZgOsYQAlN9YjES4RGgmRF8_-cL6qACLcBGAs/s320/aitoff_distortions.png"></a><br />Distortion comparison of the pseudostereographic (left) and Aitoff (right) projections.</center>

## Wiechel ellipse
The Wiechel pseudoazimuthal projection is a modification of the azimuthal equal-area projection in an attempt to make it both equal-area and equidistant. It essentially looks like a pinwheel and has some severe angular deformations because of it. Turning this into a Hammer-like map may probably still retain its area equivalence, at the cost of losing its equidistant properties and terrible angular deformations, so it's more of a novelty.

I don't wanna say "Wiechel pseudoazimuthal" for this modified version because the original one is already a pseudoazimuthal projection.

<center><a href="https://4.bp.blogspot.com/-9Zsi7TxELP0/XNCE1kqfevI/AAAAAAAAAaM/ZkCNlkuJCk8yAuNLQc-NDGHKOrBSUEh7ACLcBGAs/s0/wiechel_pseudopseudoazimuthal.png"><img src="https://4.bp.blogspot.com/-9Zsi7TxELP0/XNCE1kqfevI/AAAAAAAAAaM/ZkCNlkuJCk8yAuNLQc-NDGHKOrBSUEh7ACLcBGAs/s640/wiechel_pseudopseudoazimuthal.png"></a></center>
## Bonus: Logarithmic pseudoazimuthal
The logarithmic azimuthal is based on the azimuthal equidistant projection, designed to magnify the central portion of the map. It can also be used humorously by blowing up the central portion excessively.

<center><a href="https://1.bp.blogspot.com/-a-6iFsIJGJE/XNCCZfJ0xjI/AAAAAAAAAZc/x0RKUGvpkfkHSFQPfc-Sy7_Skj344SuSwCLcBGAs/s0/logarithmic-pseudoazimuthal_5.png"><img src="https://1.bp.blogspot.com/-a-6iFsIJGJE/XNCCZfJ0xjI/AAAAAAAAAZc/x0RKUGvpkfkHSFQPfc-Sy7_Skj344SuSwCLcBGAs/s640/logarithmic-pseudoazimuthal_5.png"></a><br />The logarithmic pseudoazimuthal projection with a cental scaling of 5.</center>

<center><a href="https://1.bp.blogspot.com/-JSdWm8VUiQY/XNCCFXJczXI/AAAAAAAAAZU/-fg-wC5tgDkDQYcd8M2wvfG5UbTM3ZCJgCLcBGAs/s0/BULGE_OWO_WHATS_THIS.png"><img src="https://1.bp.blogspot.com/-JSdWm8VUiQY/XNCCFXJczXI/AAAAAAAAAZU/-fg-wC5tgDkDQYcd8M2wvfG5UbTM3ZCJgCLcBGAs/s640/BULGE_OWO_WHATS_THIS.png"></a><br />Who says you can't have fun with map projections?</center>