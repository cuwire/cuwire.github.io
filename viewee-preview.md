---

layout: page
title: preViewEE
permalink: /viewee/preview/

---

## Check it out for github repositories:

<link rel="stylesheet" type="text/css" href="../../vieweejs/styles/font.css" />
<link rel="stylesheet" type="text/css" href="../../vieweejs/styles/style.css" />
<link rel="stylesheet" type="text/css" href="../../vieweejs/styles/browser.css" />

<script type="text/javascript" src="../../vieweejs/lib/object-assign.js"></script>
<script type="text/javascript" src="../../vieweejs/lib/minivents.js"></script>
<script type="text/javascript" src="../../vieweejs/lib/htmlel.js"></script>

<script type="text/javascript" src="../../vieweejs/lib/FontLoader.js"></script>

<script type="text/javascript" src="../../vieweejs/src/eagle_xml_parser.js"></script>
<script type="text/javascript" src="../../vieweejs/src/kicad_pcb_parser.js"></script>
<script type="text/javascript" src="../../vieweejs/src/geda_parser.js"></script>

<script type="text/javascript" src="../../vieweejs/src/renderer.js"></script>
<script type="text/javascript" src="../../vieweejs/src/canvas_renderer.js"></script>
<script type="text/javascript" src="../../vieweejs/src/svg_renderer.js"></script>

<script type="text/javascript" src="../../vieweejs/src/viewee.js"></script>

<script type="text/javascript" src="../../vieweejs/src/interface.js"></script>

<script type="text/javascript" src="../../vieweejs/src/browser.js"></script>

<div style="font-family: vector; visibility: hidden; position: absolute; opacity: .01"> </div>
<div class="viewee-wrapper">
<div class="search">
<form class="search">
<input type="text" name="searchInput" placeholder="Search for Eagle/Kicad/gEDA" />
</form>
<ul class="results">
</ul>
</div>
<div class="viewee">
<div id="hintsbox">
<p><span id="hintstitle"></span> <span id="hintstext"></span></p>
</div>
<form class="controls" style="background-color: transparent;">
<div class="split">
<input type="radio" id="side-front" value="front" name="side" checked="true"/>
<label for="side-front">Front</label>
<input type="radio" id="side-back" value="back" name="side"/>
<label for="side-back">Back</label>
</div>
<div class="split">
<button type="button" class="button zoomIn" id="zoominbutton">+</button>
<button type="button" class="button zoomOut" id="zoomoutbutton">-</button>
</div>
<div class="button dropdown" id="showlayerbutton">
Layers...
<ul class="layers">
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_5" onclick="toggleLayer(5);"/>Top Copper</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_6" onclick="toggleLayer(6);"/>Top silkscreen</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_7" onclick="toggleLayer(7);"/>Top documentation</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_1" onclick="toggleLayer(1);"/>Bottom copper</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_2" onclick="toggleLayer(2);"/>Bottom silkscreen</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_3" onclick="toggleLayer(3);"/>Bottom documentation</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_9" onclick="toggleLayer(9);"/>Outline</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_8" onclick="toggleLayer(8);"/>Vias</li>
<li><input type="checkbox" checked="checked" id="SHOW_LAYER_CB_4" onclick="toggleLayer(4);"/>Dim backside</li>
</ul>
</div>
</form>
<div class="hcenter">
<div class="vcenter">

<!--

<canvas class="canvas" width="800" height="600"></canvas>
-->
<svg class="canvas"></svg>

</div>
</div>
</div>
</div>
