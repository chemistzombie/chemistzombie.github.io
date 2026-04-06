---
layout: default
title: countdowns
---
some countdowns for potentially important dates (possible dates for signora's resurrection and playability)
<table>
<tbody>
 <tr><td><strong>Version</strong></td><td><strong>Time remaining</strong></td></tr>
 <tr><td>6.8</td><td id="68" style="font-family:monospace;"></td></tr>
 <tr><td>6.9?</td><td id="69" style="font-family:monospace"></td></tr>
 <tr><td>7.1/7.2</td><td id="72" style="font-family:monospace"></td></tr>
</tbody></table>

<script>
var dateOne = new Date("Aug 12, 2026 09:00:00").getTime();
var dateTwo = new Date("Sep 23, 2026 09:00:00").getTime();
var dateThree = new Date("Dec 16, 2026 09:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distanceOne = dateOne - now;
    
  // Time calculations for days, hours, minutes and seconds
  var daysOne = Math.floor(distanceOne / (1000 * 60 * 60 * 24));
    
  // Output the result in an element with id="demo"
  document.getElementById("68").innerHTML = daysOne + " days";
  // If the count down is over, write some text 
  if (distanceOne < 0) {
    clearInterval(x);
    document.getElementById("68").innerHTML = "EXPIRED";
  }
}, 1000);

var y = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distanceTwo = dateTwo - now;
    
  // Time calculations for days, hours, minutes and seconds
  var daysTwo = Math.floor(distanceTwo / (1000 * 60 * 60 * 24));
    
  // Output the result in an element with id="demo"
  document.getElementById("69").innerHTML = daysTwo + " days";
  if (distanceTwo < 0) {
    clearInterval(y);
    document.getElementById("69").innerHTML = "EXPIRED";
  }
}, 1000);

var z = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distanceThree = dateThree - now;
    
  // Time calculations for days, hours, minutes and seconds
  var daysThree = Math.floor(distanceThree / (1000 * 60 * 60 * 24));
    
  // Output the result in an element with id="demo"
  document.getElementById("72").innerHTML = daysThree + " days";
  if (distanceThree < 0) {
    clearInterval(z);
    document.getElementById("72").innerHTML = "EXPIRED";
  }
}, 1000);
</script>
