# Plotly #

### What is this repository for? ###

* Basic examples of Plotly.js
* 1.29.3
* [Learn Plotly.js](https://plot.ly/javascript/getting-started/)

### How do I get set up? ###

* What is plotly.js?

	Built on top of d3.js and stack.gl, plotly.js is a high-level, declarative charting library. plotly.js ships with 20 chart types, including 3D charts, statistical graphs, and SVG maps. 

* Getting Started with plotly.js

	Download
	
		Download the minified plotly.js source code and dependencies.
		Include the downloaded scripts before the end of the </head> tag in your HTML document:
			
			<head>
				<script src="plotly-latest.min.js"></script>
			</head>
	
	Start plotting!

		In your HTML document, create an empty DIV to draw the graph in:

			<div id="tester" style="width:600px;height:250px;"></div>

		Now you can make interactive plotly.js charts using Plotly.plot().

			<script>
				TESTER = document.getElementById('tester');
				Plotly.plot( TESTER, [{
				x: [1, 2, 3, 4, 5],
				y: [1, 2, 4, 8, 16] }], {
				margin: { t: 0 } } );
			</script>

### Example ###

* Basic example to plot a line graph

	<html>
    	<head>
        	<title>Basic Line Plot</title>
    	</head>
    	<body>
        	<div id="myDiv"><!-- Plotly chart will be drawn inside this DIV --></div>
        	<script src="/web/assets/js/plotly-latest.min.js"></script>
        	<script>
            	var trace1 = {
            	x: [1, 2, 3, 4], 
            	y: [10, 15, 13, 17], 
            	type: 'scatter'
            	};
            	var trace2 = {
            	x: [1, 2, 3, 4], 
            	y: [16, 5, 11, 9], 
            	type: 'scatter'
            	};
            	var data = [trace1, trace2];
            	var layout = {
            	title:'Basic Line Plot'
            	};
            	Plotly.newPlot('myDiv', data, layout);
        	</script>
    	</body>
	</html>

        



### Who do I talk to? ###

* Mitesh Banka
	banka.mitesh@gmail.com
	+91-8482096370