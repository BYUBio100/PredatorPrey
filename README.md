# PredatorPrey
<!DOCTYPE HTML>
<html>
<head>
	<title>Predator / Prey Simulation</title>
	<link rel="stylesheet" type="text/css" href="css/styles.css"> 
	<link rel="stylesheet" type="text/css" href="css/jquery-ui.css"> 
	<script type="text/javascript" src="scripts/jquery.js"></script>
	<script type="text/javascript" src="scripts/jquery-ui.js"></script>
	<script type="text/javascript" src="scripts/AnimalModel.js"></script>
	<script type="text/javascript" src="scripts/Graph.js"></script>
	<script type="text/javascript" src="scripts/DataSet.js"></script>
	<script type="text/javascript" src="scripts/LotkaVolterra.js"></script>
	<script type="text/javascript" src="scripts/Point.js"></script>
	<script type="text/javascript" src="scripts/Main.js"></script>
</head>
<body>
    <div id="wrapper">
		<div id="options">
			<table id="model-parameters">
				<tr><td id="prey-heading" class="heading" colspan="3">Prey</td></tr>
				<tr>
					<td colspan="2">Initial Population:</td>
					<td><input type="text" id="prey-initial-population" class="param" value="500"/></td>
				</tr>
				<tr>
					<td>Growth rate:</td>
					<td><div id="prey-growth-slider" class="slider"></div></td>
					<td><input type="text" id="prey-growth-rate" class="param"/></td>
				</tr>
				<tr>
					<td>Death rate:</td>
					<td><div id="prey-death-slider" class="slider"></div></td>
					<td><input type="text" id="prey-death-rate" class="param"/></td>
				</tr>

				<tr><td id="predator-heading" class="heading" colspan="3">Predator</td></tr>
				<tr>
					<td colspan="2">Initial Population:</td>
					<td><input type="text" id="predator-initial-population" class="param" value="20"/></td>
				</tr>
				<tr>
					<td>Growth rate:</td>
					<td><div id="predator-growth-slider" class="slider"></div></td>
					<td><input type="text" id="predator-growth-rate" class="param"/></td>
				</tr>
				<tr>
					<td>Death rate:</td>
					<td><div id="predator-death-slider" class="slider"></div></td>
					<td><input type="text" id="predator-death-rate" class="param"/></td>
				</tr>

				<tr><td id="advanced-heading" class="heading" colspan="3">Simulation Options</td></tr>
				<tr>
					<td colspan="2">Generations:</td>
					<td><input type="text" id="generations" class="param" value="1000"/></td>
				</tr>
				<tr>
					<td colspan="2">Time Step:</td>
					<td><input type="text" id="time-step" class="param" value=".01"/></td>
				</tr>
				<tr>
					<td colspan="3" id="compare-to-td"><input type="checkbox" id="compare-to-checkbox" value="compare" />Compare to previous?</td>
				</tr>
				<tr>
					<td colspan="3"><input type="button" id="simulate-button" value="Simulate" /></td>
				</tr>

			</table>
		</div>
		<div id="graph">
			<div id="canvas-div" width="560" height="450">
				
			</div>
			<div id="save-graph">
				<a href="#" onclick="saveGraph()">Save Graph</a>
				<p><em>Click the link above to open a window with the image.  Then, right-click and click "Save image as..." to save to your computer.</em></p>
			</div>
		</div>
	</div>

</body>
</html>
