---
layout: default
title: Fi
---

Hello ;) world :) :( :( :(

<script type="text/javascript">
 
    var emoticons = {
        ':)'         : '/images/u.gif',
        ':('         : 'sad.gif',
        ';)'         : 'wink.gif'


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