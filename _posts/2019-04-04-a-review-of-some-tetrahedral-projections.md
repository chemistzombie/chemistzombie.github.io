# Tetrahedral projections
## AuthaGraph
Pros:
* Minimum-error projection: balances out areal and angular distortions to an acceptable degree.
* Good placement of landmasses to avoid severe distortions.

Cons:
* Its equations is proprietary and has never been published anywhere, requiring people to resort to alternatives such as its reverse-engineered clone to make similar maps.
* Because of the above reason, it's impossible to use the original projection in any GIS software.
* Landmasses such as Australia or Brazil look weird with this projection.
* Compromise projection means that it's not really equal-area as it name claims it to be.

## Lee tetrahedral
Pros:
* Very good conformal projection: preserves angles locally while maintaining area proportions relatively well unlike most conformal projections. A good configuration of the map can yield you results where most landmasses avoid touching the singularities, where its conformality is lost and distortions are the worst.
* The AuthaGraph-like configuration is a good example of this.
* Generally looks more appealing than conformal or equal-area tetrahedral projections due to its angle-preserving nature, and landmasses look more normal.

Cons:
* Higher area distortion than compromise projections, although this is to be expected.

## van Leeuwen
Pros:
* Equal-area: absolutely no areal distortions unlike AuthaGraph.
* Using the AuthaGraph-like configuration also yield pretty good results to minimize its angular distortions.

Cons:
* Severe angular deformations are noticeable with this projection, though this is to be expected due to its authalic properties.
* Landmasses look even weirder than AuthaGraph because of this.

## Kunimune's "EquaHedral"
Pros:
* Interrupted equal-area: Minimizes distortions that is caused by its area equivalence properties, resulting in a better looking map than van Leeuwen.
* Customizable: Sinus length can be adjusted to suit the user's needs

Cons:
* Interruptions make it difficult to measure distances in certain cases, and can slice up landmasses.
* Its best configuration with sinus length of 42 isn't compatible with the AuthaGraph-like positioning of landmasses, since it slices up Brazil, Russia, and Indonesia.
## Kunimune's "TetraGraph"