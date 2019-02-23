---
layout: default
title: GTA SA alternative cheat codes (rewrite)
---

# GTA SA alternative cheat codes
These cheat codes were found using this tool. As far as I'm aware, it's the only working cheat code finder that's available on the internet, so huge thanks to its author.

## Notes
The ␣ symbol denotes spaces.

Intended cheat code is essentially what the developers intended you to input if you wanted to activate the cheat code. For a long time, these codes remained a mystery: back in 2005, a user on GTAForums named edisoncarter as well as some other users attempted to find these intended codes. However, most of those were still missing since the dictionary attack they used was flawed: First, it used a dictionary taken from the american.gxt file of the game, as opposed to something better such as the official Scrabble dictionary. Not only that, they didn't consider the possibility that the intended cheat codes can be longer than five words and range anywhere between 6-24 characters. Eventually, they all just gave up after failing to find a lot of them and moved on with their lives. It wasn't until almost 10 years later that all the intended cheat codes were found, thanks to the release of the Android version of GTA SA, where a GTAForums user named Alexander Blade found a file that contains them there.

Shortest codes are the codes that contain the least amount of characters possible. This is split into two:
The first one is the shortest code with combinations of A-Z, 0-9, and spacebar. This should work on any keyboard layout.
The other one is the shortest code with combinations of A-Z, 0-9, spacebar, and symbols found in US QWERTY keyboards, excluding those that require holding the Shift key (because those don't work).
With this combination, it appears that all the cheat codes except for the sandstorm weather cheat can hit 6 characters long, further improving the length, but be aware that oftentimes this only works with US QWERTY keyboards due to the placements of the keys, and while these codes might be much shorter than the other combos, it doesn't necessarily mean that you can type it faster. Some of these symbols can be difficult to reach and/or memorize.


I've managed to download edisoncarter's cheat codes dumps he published on his site back then using Wayback Machine. You can find them here:
Two-word cheats dump
Three-word cheats dump, sorted by length
Three-word cheats dump, sorted by cheat index number
Four-word cheats dump, 13 letters only
Nine-letter cheats dump

It's highly recommended to not save the game after using cheats, as some of them, such as the riot cheat code, can't be disabled and can cause severe glitches such as the infamous "Madd Dogg glitch". However, some of them, such as weapon, health, wanted level, and spawn vehicle cheat codes appear to have no side effects to the save file, so those are probably safe to use.

<script type="text/javascript">
 
    var emoticons = {
        ':1:'   : '/images/l1.gif',
        ':2:'   : '/images/l2.gif',
        ':3:'   : '/images/r1.gif',
		':4:'	: '/images/r2.gif',
		':u:'   : '/images/u.gif',
        ':d:'   : '/images/d.gif',
        ':l:'   : '/images/l.gif',
		':r:'	: '/images/r.gif',
		':t:'   : '/images/t.gif',
        ':s:'   : '/images/s.gif',
        ':c:'   : '/images/c.gif',
		':x:'	: '/images/x.gif',
		':l1:'	: '/images/l1.gif',
        ':l2:'	: '/images/l2.gif',
        ':r1:'	: '/images/r1.gif',
		':r2:'	: '/images/r2.gif',
		':L1:'	: '/images/l1.gif',
        ':L2:'	: '/images/l2.gif',
        ':R1:'	: '/images/r1.gif',
		':R2:'	: '/images/r2.gif',
		':U:'   : '/images/u.gif',
        ':D:'   : '/images/d.gif',
        ':L:'   : '/images/l.gif',
		':R:'	: '/images/r.gif',
		':T:'   : '/images/t.gif',
        ':S:'   : '/images/s.gif',
        ':C:'   : '/images/c.gif',
		':X:'	: '/images/x.gif'
    }

document.querySelectorAll('p').forEach(e => e.innerHTML = replaceEmoticons(e.innerHTML, emoticons));

function replaceEmoticons(text, emotes) {
   return Object.keys(emotes).reduce((result, emote) => {
      return result.replace(new RegExp(RegExpEscape(emote), 'gi'), function(match) {
        return (img => img != null ? '<img src="' + img + '"/>' : match)(emotes[match]);
      });
    }, text);
}

// helper function to escape special characters in regex
function RegExpEscape(text) {
  return text.replace(/[-[\]{}()*+?.,\\^$|#\s]/g, "\\$&");
}

// Map emote ids to their URLs.
function mapIdsToPaths(emotes, url, prefix, size) {
  Object.keys(emotes).forEach((id) => {
    emotes[id] = url + prefix + emotes[id] + '-' + size + '.png';
  });
}

</script>