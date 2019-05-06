# Tetrahedral projections

## AuthaGraph
<center><a href="/images/AuthMapHP3.jpg"><img src="/images/AuthMapHP3.jpg"></a></center>
<center><a href="https://chemistzombie.files.wordpress.com/2019/04/autha.png"><img src="https://chemistzombie.files.wordpress.com/2019/04/autha.png?w=1024"></a><br /><span style="font-size:10pt">Top: The official AuthaGraph map<br />Above: The projection's clone applied to a silhouette map of the Earth</span></center>

Pros:
* Minimum-error projection: balances out areal and angular distortions to an acceptable degree.
* Good placement of landmasses to avoid severe distortions.
* Won the Japanese Good Design Grand Award in 2016.
* Probably the most well-known tetrahedral projection out of all after it took the media by storm.

Cons:
* Its equations is proprietary and has never been published anywhere, requiring people to resort to alternatives such as its [reverse-engineered clone](https://kunimune.home.blog/2017/11/23/the-secrets-of-the-authagraph-revealed/) to make similar maps.
	* Because of this, it's impossible to use the original projection in any GIS software.
	* Not only that, every single image of this projection on the internet uses THE SAME SHITTY ~~LOW-RESOLUTION~~ POLITICAL MAP, WHICH IS THE ONLY MAP THEY WERE WILLING TO PUBLISH ON THEIR WEBSITE (see above). **UPDATE**: I've managed to find a high resolution image of the map. See here.
* Landmasses such as Australia or Brazil look weird with this projection despite the its minimum-error properties.
* Compromise projection means that it's not really equal-area as it name claims it to be.

## Lee tetrahedral
<center><a href="https://chemistzombie.files.wordpress.com/2019/04/leetetra-authagraph.png"><img src="https://chemistzombie.files.wordpress.com/2019/04/leetetra-authagraph.png?w=1024"></a></center>

Pros:
* One of the best conformal projections: preserves angles locally while maintaining area proportions relatively well unlike most conformal projections. A good configuration of the map can yield results where most landmasses avoid touching the singularities, where its conformality is lost and distortions are the worst.
	* The AuthaGraph-like configuration is a good example of this.
* Unlike most conformal projections, it's possible to show the entire world with this projection, and it tessellates too.
* Generally looks more appealing than compromise or equal-area tetrahedral projections due to its angle-preserving nature, and landmasses look more "normal".

Cons:
* Higher area distortion than compromise projections, although this is to be expected.
	* This causes Western Australia to appear noticeably inflated.
* As with most conformal projections, singularities do exist on the edges of the map.

## van Leeuwen
Pros:
* Equal-area: absolutely no areal distortions unlike AuthaGraph.
* Using the AuthaGraph-like configuration also yield pretty good results to minimize its angular distortions.

Cons:
* Severe angular deformations are noticeable with this projection, though this is to be expected due to its authalic properties.
* Landmasses look even weirder than AuthaGraph because of this.

## Kunimune's "EquaHedral"
<center><a href="https://chemistzombie.files.wordpress.com/2019/04/equahedral-authagraph.png"><img src="https://chemistzombie.files.wordpress.com/2019/04/equahedral-authagraph.png?w=1024"></a></center>
Pros:
* Interrupted equal-area: Minimizes distortions that is caused by its area equivalence properties, resulting in a better looking map than van Leeuwen.
* Customizable: Sinus length can be adjusted.

Cons:
* Interruptions make it difficult to measure distances in certain cases, and can slice up landmasses.
* Its best configuration with sinus length of 42 isn't compatible with the AuthaGraph-like positioning of landmasses, since it slices up Brazil, Russia, and Indonesia.

## Kunimune's "TetraGraph"
<center><a href="https://chemistzombie.files.wordpress.com/2019/04/tetragraph-authagraph.png"><img src="https://chemistzombie.files.wordpress.com/2019/04/tetragraph-authagraph.png?w=1024"></a></center>
