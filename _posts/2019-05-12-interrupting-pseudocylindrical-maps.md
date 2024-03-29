# Interrupting pseudocylindrical maps
It turns out that most, if not all, pseudocylindrical and similar types of maps can be interrupted. NASA's G-Projector software supports interruptions of some pseudocylindrical projections (Goode homolosine, Mollweide, Sinusoidal) but unfortunately doesn't offer it for most other pseudocylindrical projections. For example, the McBryde P3, which is based on Craster parabolic projection can be interrupted (and is in interrupted format by default), but the original parabolic projection itself can't.

I looked up for a way to interrupt these projections myself and found [this answer](https://gis.stackexchange.com/a/1798) on Stack Exchange. It basically requires an image editing tool (I used Photoshop) and a bit of patience. I'll just put it here for convenience:

> If you look at a random example of the interrupted sinusoidal, each perfectly vertical meridian corresponds to a single sinusoidal projection.
>
> For that example, you're looking at sinusoidals centered on longitudes: -160,-100,-60, ...
>
> Then, cut and shift the parts to line up: The bottom left part is composed of longitudes -180..-100 and latitudes 0..-90, and projected with a center longitude of -160. The next part is longitudes -180..-40 and latitudes 0..90, projected w/ a center of -100. And so on (the example I linked was pretty intricate & there might be funny business going on in Russia; it doesn't look like a vanilla sinusoidal there).

It doesn't have to be sinusoidal; any pseudocylindrical, lenticular and other similar projections can be used, such as the Robinson or Hammer projection. However, it's best to use a projection that has a straight equatorial line to make it easier to cut the north and south parts. The projection also doesn't need to be equal area; while most of the commonly used interrupted projections are equal area (e.g. Goode homolosine), compromise projections (e.g. Winkel tripel) can still be used, resulting in an even more minimum-error map.

The rule of thumb is, if both the central parallel and meridian are straight, and the widest part of the projection is on the center, then it's most likely interruptible.

Before proceeding to the manually created examples, let's see all the projections that can be interrupted by G.Projector.

# G.Projector interrupted maps
## Boggs eumorphic
The Boggs eumorphic projection is an arithmetic mean of the sinusoidal and Mollweide projections. The difference between this projection and the Goode homolosine is that this one is an average of the two projections, while the latter is simply a fusion of them.

The name "eumorphic" means "good shape"
## Baker dinomic
The Baker dinomic projection is a fusion of the Mercator and sinusoidal projections at 45°, with interruptions only on the sinusoidal projection.

## Goode homolosine
The Goode homolosine is a fusion of the sinusoidal and Mollweide projections at 40°44'11.98'' (approx. 40.737°). The projection was originally copyrighted but then expired, because it's not possible to copyright mathematical designs in the US, map projections included.

The name itself is a portmanteau of "homolographic" (Mollweide's alternative name) and "sine".

Oddly enough, the Goode homolosine uses the uninterrupted format by default despite it being rarely shown that way.

## McBryde projections
F. Webster McBryde developed a series of equal-area projections for use in interrupted maps. These projections are patented, but the equations are publicly available, owing to the inability of copyrighting mathematical designs in the US. G.Projector offers all of them in the software, and they use McBryde's landmasses interruption patterns by default, although other interruption methods (including the McBryde oceans interruptions) and uninterrupted maps are available.

An older projection series also exists under the name of McBryde-Thomas flat polar projections.

The following maps use Goode's interruption patterns for consistency.

## McBryde P3
The McBryde P3 is a fusion of the Craster parabolic (hence the P designation) and McBryde-Thomas flat polar parabolic projections at 49°20' (approx. 49.333°)

While this projection contains portions of the Craster parabolic projection and can be interrupted in G.Projector, the original Craster parabolic itself can't, for some reason.
## McBryde Q3
The McBryde Q3 is a fusion of the quartic authalic (Q designation) and McBryde-Thomas flat polar quartic projections at 52°09' (52.15°).

## McBryde S2
The McBryde S2 is a fusion of the sinusoidal (S designation) and Eckert VI at 49°16' (approx. 49.267°).

## McBryde S3
The McBryde S3 is a fusion of the sinusoidal and McBryde-Thomas flat-polar sinusoidal at 55°51' (55.85°). Interestingly, whoever wrote the G.Projector user's manual doesn't seem to know the second projection of this, replacing it with "???" instead.

## McBryde-Thomas flat polar parabolic

## McBryde-Thomas flat polar quartic

## McBryde-Thomas flat polar sinusoidal

## Mollweide
The Mollweide

For some reason, this projection is interrupted by default, using Goode's interruption patterns (i.e. the Goode interrupted Mollweide). This projection is normally presented in an uninterrupted format, and it's rather weird that the developers of the software chose the interrupted one as the default.

## Quartic authalic
The quartic authalic projection is an equal area projection first invented by Karl Siemon in 1937 under the name of Siemon III, but was reintroduced by Oscar S. Adams in 1944, commenting that "as far as we know, no such projection has been heretofore proposed." It was named so due to its fourth-order curves.

## Siemon IV
The Siemon IV projection is a modification of the quartic authalic with axes adjusted to a 2:1 ratio by dividing x-values and multiplying y-values by 1.05391. 

## Sinusoidal

# Examples of manually interrupted maps
## Craster parabolic

## Equal Earth
The Equal Earth projection is a new pseudocylindrical equal-area projection designed by Bojan Savric, Tom Patterson and Bernhard Jenny in 2018, and was inspired by the Eckert IV and Robinson projection. It was made in response to the adoption of the Gall-Peters map by Boston public schools and serves as a visually appealing alternative to it.

This example uses the Goode interruption pattern (displayed as "Interrupted: Continents" in G.Projector), but any interruptions can be used.

<center><a href="https://1.bp.blogspot.com/-TahxeZQdPOE/XMfEpvdMd3I/AAAAAAAAAXc/Z5vP4kk8XXkmroOC76Amx81G6D3_USjEQCLcBGAs/s0/equalearth-goode-unextended.png"><img src="https://1.bp.blogspot.com/-TahxeZQdPOE/XMfEpvdMd3I/AAAAAAAAAXc/Z5vP4kk8XXkmroOC76Amx81G6D3_USjEQCLcBGAs/s640/equalearth-goode-unextended.png"></a><br />Interrupting this map reveals a substantial vertical stretching on low- and mid-latitude regions.</center>

## Fahey
The Fahey projection is a modification of the cylindrical stereographic projection designed by Lawrence Fahey in 1975.  The parallels are spaced for a Gall stereographic based on a cylinder secant at about 35° instead of 45°, making it closer to the less-known BSAM cylindrical, which uses a standard parallel of 30°.

This example uses the Baker interruption pattern, which is used for the Baker dinomic projection.

<center><a href="https://3.bp.blogspot.com/-RStgjpPgPJA/XMfUuXLa0cI/AAAAAAAAAX0/DsZ_tTH8dlkxPZdsF_9lv-PlJXOsZGsywCLcBGAs/s0/fahey-baker.png"><img src="https://3.bp.blogspot.com/-RStgjpPgPJA/XMfUuXLa0cI/AAAAAAAAAX0/DsZ_tTH8dlkxPZdsF_9lv-PlJXOsZGsywCLcBGAs/s640/fahey-baker.png"></a><br /></center>

## Foucaut stereographic equivalent
The Foucaut stereographic equivalent is a novelty equal-area map projection, named so because the spacing of the parallels along the central meridian
is the same as that of the equatorial stereographic azimuthal projection (or of Braun's stereographic cylindrical). It has very sharp poles and much more extreme shearing in the polar regions than that of the sinusoidal, so it's essentially useless for general-purpose maps.

<center><a href="https://2.bp.blogspot.com/-4kS2KhOSJxs/XNcVsdqHSuI/AAAAAAAAAdY/k4dlVTgROKMx-EcRM6KXLKt0knnhNgjdQCLcBGAs/s0/foucaut-goode.png"><img src="https://2.bp.blogspot.com/-4kS2KhOSJxs/XNcVsdqHSuI/AAAAAAAAAdY/k4dlVTgROKMx-EcRM6KXLKt0knnhNgjdQCLcBGAs/s640/foucaut-goode.png"></a><br />The Foucaut stereographic equivalent projection with Goode interruption pattern. Clearly, not even interruptions can help save this map from being really distorted.</center>

## Larrivee
The Larrivee projection somewhat resembles Van der Grinten I in terms of maintaining distortions but has somewhat less distortion and no circular arcs. The poles are also of curved lines.

<center><a href="https://2.bp.blogspot.com/-Hir9oexQ0cY/XNcWUP97-vI/AAAAAAAAAdg/aaDXnpNsjMkk2pg9FPEiIaLihh8a5ANTQCLcBGAs/s0/larrivee-mcbryde.png"><img src="https://2.bp.blogspot.com/-Hir9oexQ0cY/XNcWUP97-vI/AAAAAAAAAdg/aaDXnpNsjMkk2pg9FPEiIaLihh8a5ANTQCLcBGAs/s640/larrivee-mcbryde.png"></a><br />The Larrivee projection with McBryde interruption pattern. Because the poles are curved inwards, each lobes have different pole sizes.</center>

## Loximuthal
The loximuthal projection is a compromise projection that was designed so that straight lines from a chosen center are loxodromes or rhumb lines of true length, path, and direction from the center. Its reference (central) latitude is adjustable to the user's needs.

The easiest method of interrupting a loximuthal projection is to set the reference latitude at the equator, which makes it look similar to the Bordone oval projection. Setting the reference latitude to anything other than 0 degrees will cause the interrupted maps to overlap, requiring some readjustments to make it look right (that is, using the negative reference latitude as the interruption center.

<center><a href="https://1.bp.blogspot.com/-cNjNmZxos3Y/XNcQ5-8Dc3I/AAAAAAAAAcw/XMDMXAgyI4QaVohMLP5sQiewgk6PhuykgCLcBGAs/s0/loximuthalGoode.png"><img src="https://1.bp.blogspot.com/-cNjNmZxos3Y/XNcQ5-8Dc3I/AAAAAAAAAcw/XMDMXAgyI4QaVohMLP5sQiewgk6PhuykgCLcBGAs/s640/loximuthalGoode.png"></a><br />The "Bordone oval" loximuthal projection, with Goode interruption pattern.</center>

<center><a href="https://2.bp.blogspot.com/-fVuDw9rAxm8/XNcUPaj2iNI/AAAAAAAAAdM/zGwFroOlfeMBK4Tvvxg5vA2H8iOk1esKQCEwYBhgL/s1600/45nloximuthal-baker.png"><img src="https://2.bp.blogspot.com/-fVuDw9rAxm8/XNcUPaj2iNI/AAAAAAAAAdM/zGwFroOlfeMBK4Tvvxg5vA2H8iOk1esKQCEwYBhgL/s640/45nloximuthal-baker.png"></a><br />This is what happens if you try to interrupt a loximuthal projection that isn't centered on the equator. Notice the odd curves at the lower portions of the map. Fixing this requires readjusting the interruption center, which should be at 45 degrees south in this case.</center>

## Kavrayskiy VII
The Kavrayskiy VII projection is a minimum-error compromise pseudocylindrical projection. It balances areal and angular distortions to an acceptable level, just like Robinson and Winkel tripel. However, it's very rarely used outside of Russia and former Soviet Union countries.

Compared to Robinson and Winkel tripel, Kavrayskiy VII has very simple equations, which is amazing considering how it's on par with those two projection in reducing distortions.

## Mayr
The Mayr projection is a pseudocylindrical equal-area projection. The computation of one of Mayr’s projection equations depends on the solution of an elliptical integral, which likely contributes to its minimal use today (such things are supposedly slow to calculate on computers). In 2008, Ipbuker has proposed [alternative solutions](https://www.tandfonline.com/doi/abs/10.1559/152304008784864659) to generate it, utilizing analytical expressions.



## Ortelius oval
I know that literally no one uses this very old projection, but this one is interesting because although it appears to be a pseudocylindrical projection, it doesn't qualify as one because the meridians are not equally spaced along the parallels, so it doesn't belong to any common types of projection. If I had to name what kind of projection this is, I'd say it's a "pseudopseudocylindrical projection".	

<center><a href="https://2.bp.blogspot.com/-0ybNZqncwQU/XMnquVFErRI/AAAAAAAAAYo/lLNdBopGUUcQIsMB2SmWpSRniZPikdqVQCLcBGAs/s0/ortel-baker.png"><img src="https://2.bp.blogspot.com/-0ybNZqncwQU/XMnquVFErRI/AAAAAAAAAYo/lLNdBopGUUcQIsMB2SmWpSRniZPikdqVQCLcBGAs/s640/ortel-baker.png"></a><br />This actually looks pretty neat for an obsolete projection.</center>

## Van der Grinten I
The Van der Grinten is a compromise projection with a circular shape, used by the Nat Geo from 1922 to 1988, when it was replaced by the Robinson projection. It was designed to combine the appearance of Mercator while having a rounded shape like Mollweide. This projection is normally cropped near the poles on world maps due to its extreme distortion there, although it's able to show the entire world.

A circular projection that's actually conformal exists, and is named the Lambert-Lagrange projection, which was apparently developed earlier than Van der Grinten, although it was unfortunately never popular, and is such an underrated projection. If I were to choose between Van der Grinten and Lambert-Lagrange, I'd definitely pick the latter due to its ability to show the entire world while maintaining conformality just like Mercator, which makes it superior. It's essentially the Van der Grinten successor that never was.

<center><a href="https://1.bp.blogspot.com/-NkVdbsC-kVQ/XNcVPoL6TCI/AAAAAAAAAdQ/ommYkz8w8f43B1E1HnHJ0uy4P0uYhhpNgCLcBGAs/s0/vdg-mcbryde.png"><img src="https://1.bp.blogspot.com/-NkVdbsC-kVQ/XNcVPoL6TCI/AAAAAAAAAdQ/ommYkz8w8f43B1E1HnHJ0uy4P0uYhhpNgCLcBGAs/s640/vdg-mcbryde.png"></a><br />The Van der Grinten projection with McBryde interruption pattern. It does help make the map slightly more "conformal".</center>

## Winkel tripel
Here's something you might have been waiting for: the Winkel tripel projection, now in interrupted form. If you like Nat Geo's preferred compromise projection, you better see this.

<center><a href="https://1.bp.blogspot.com/-QhegUUdL8ZY/XMnhskckm1I/AAAAAAAAAYM/PYYO7IM9p4oAy5nhUt0Vk9UVt_xtBVxRQCLcBGAs/s0/winkel-goode.png"><img src="https://1.bp.blogspot.com/-QhegUUdL8ZY/XMnhskckm1I/AAAAAAAAAYM/PYYO7IM9p4oAy5nhUt0Vk9UVt_xtBVxRQCLcBGAs/s640/winkel-goode.png"></a><br />Looks nice.</center>

## Robinson
Another excellent minimum-error projection in interrupted form. To be honest it looks better than the interrupted Winkel tripel.

<center><a href="https://1.bp.blogspot.com/-FKZRUBQhSGQ/XMnqkI_MB_I/AAAAAAAAAYk/9Cg2Vha2U2cHRLsSC5iZPpRZtE4AFiR0ACLcBGAs/s0/robinson-goode.png"><img src="https://1.bp.blogspot.com/-FKZRUBQhSGQ/XMnqkI_MB_I/AAAAAAAAAYk/9Cg2Vha2U2cHRLsSC5iZPpRZtE4AFiR0ACLcBGAs/s640/robinson-goode.png"></a><br />I prefer Robinson because it's got less vertical stretching on the low- and mid-latitude regions</center>

# Other projections that are interruptible
## Azimuthal equidistant projection
Azimuthal equidistant is the only azimuthal projection that can be interrupted. This comes at the cost of having more severe stretching on regions farther from the center.

Other azimuthal projections can't be interrupted because the spacing between each meridians aren't equal.

<center><a href="https://3.bp.blogspot.com/-BEVrKvwN4Ic/XNcK3vkyNGI/AAAAAAAAAcM/00Lw6Jtm8bUupN0ioY66Rig7tLVaV1nTgCLcBGAs/s0/azimeqdgoode.png"><img src="https://3.bp.blogspot.com/-BEVrKvwN4Ic/XNcK3vkyNGI/AAAAAAAAAcM/00Lw6Jtm8bUupN0ioY66Rig7tLVaV1nTgCLcBGAs/s640/azimeqdgoode.png"></a><br />An interrupted azimuthal equidistant projection with Goode interruption pattern.</center>

## Polyconic projections
Polyconic projections can be interrupted and might slightly resemble the interrupted azimuthal equidistant projection in certain cases. It also suffers from extreme stretching on regions farther from the center. An advantage of interrupted polyconic projections over the azimuthal projections is that the regions near the central meridian of such projections usually have little to no distortions—a trait found on the sinusoidal projection—which allow for creation of minimum error gore maps suitable for making globes. The American polyconic is an example of a projection having such traits.

<center><a href="https://3.bp.blogspot.com/-t2ZzActvobY/XNcJkBHWwVI/AAAAAAAAAcA/0mxhIH36F3sSEY-0L7BS_cKkBqLt8nMpQCLcBGAs/s0/polyconic-goode.png"><img src="https://3.bp.blogspot.com/-t2ZzActvobY/XNcJkBHWwVI/AAAAAAAAAcA/0mxhIH36F3sSEY-0L7BS_cKkBqLt8nMpQCLcBGAs/s640/polyconic-goode.png"></a><br />An interrupted American Polyconic projection, with Goode interruption pattern. Notice the severe distortions along the eastern hemisphere and the extreme stretching of the northern portions of Borneo, Sumatra and Celebes.</center>

Other examples of interrupted polyconic projections are presented below.

### Maurer SNo. 160 "Apparent Globular"
The Maurer Apparent Globular projection is one of the three polyconic projections presented by Hans Maurer. Unlike the American Polyconic projection, the Apparent Globular projection can be used to map the entire world without introducing severe distortions.

### Canters W20
The Canters W20 projection is a polyconic projection introduced by Frank Canters in 2002.

