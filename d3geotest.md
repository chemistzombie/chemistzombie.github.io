<script src="https://d3js.org/d3.v4.min.js">
<script src="https://d3js.org/d3-array.v1.min.js"></script>
<script src="https://d3js.org/d3-geo.v1.min.js"></script>
<script src="https://d3js.org/d3-geo-projection.v2.min.js"></script>

  <svg width="200" height="150">
    <rect x="0" width="15" fill="#d1c9b8"></rect>
    <rect x="5" width="15" fill="#d1c9b8"></rect>
    <rect x="10" width="15" fill="#d1c9b8"></rect>
    <rect x="15" width="15" fill="#d1c9b8"></rect>
	<rect x="20" width="15" fill="#d1c9b8"></rect>
	<rect x="25" width="15" fill="#d1c9b8"></rect>
    <rect x="30" width="15" fill="#d1c9b8"></rect>
    <rect x="35" width="15" fill="#d1c9b8"></rect>
    <rect x="40" width="15" fill="#d1c9b8"></rect>
	<rect x="45" width="15" fill="#d1c9b8"></rect>
	<rect x="50" width="15" fill="#d1c9b8"></rect>
    <rect x="55" width="15" fill="#d1c9b8"></rect>
    <rect x="60" width="15" fill="#d1c9b8"></rect>
    <rect x="65" width="15" fill="#d1c9b8"></rect>
	<rect x="70" width="15" fill="#d1c9b8"></rect>
	<rect x="75" width="15" fill="#d1c9b8"></rect>
    <rect x="80" width="15" fill="#d1c9b8"></rect>
    <rect x="85" width="15" fill="#d1c9b8"></rect>
    <rect x="90" width="15" fill="#d1c9b8"></rect>
	<rect x="95" width="15" fill="#d1c9b8"></rect>
  </svg>
<script>

var aitoff = [10,20,30,40,50,60,70,80,90,100,100,90,80,70,60,50,40,30,20,10];

d3.selectAll('rect')
  .data(aitoff)
  .attr('height', function(d){
    return d/10 * 5.5;
  })
  .attr('y', function(d){
    return 150 - d/10 * 5.5;
  });
	
</script>