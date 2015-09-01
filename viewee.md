---

layout: page
title: ViewEE
permalink: /viewee/

---

ViewEE is a software to view PCB layouts in various formats. Currently supported are Cadsoft Eagle .brd
and Kicad .kicad_pcb formats.

###Issues

Parser and renderer are not ideal. At current stage you will definitely face problem with arcs,
text alignment and thru hole pad shapes. Kicad is tested on three `.kicad_pcb` files only and probably
there is more problems than with eagle format.

###Mac OS X QuickLook plugin

You can install preview version of ViewEE for Mac OS X by downloading QuickLook plugin
from [releases page](https://github.com/cuwire/viewee/releases).

Download, unarchive, copy `.qlgenerator` file to the `~/Library/QuickLook/` folder.

####Video

<div class="videoWrapper ViewEE-QuickLook">
    <!-- Copy & Pasted from YouTube -->
    <iframe width="100%" height="315" src="https://www.youtube.com/embed/ihnCz3UOc7Y" frameborder="0" allowfullscreen></iframe>
</div>

###Library

Also you can use a javascript parser and renderer on your own page. Here is [an example](/viewee-source/) and [repository](https://github.com/cuwire/viewee/).

##Thanks

Huge thanks to people who created the original version
for [Eagle board viewer](https://github.com/presseverykey/everywhere-eagle-viewer)
and inspired me to [fix some bugs](https://github.com/presseverykey/everywhere-eagle-viewer/issues/3) and create derived software.


{% include disqus.html disqus_identifier=page.disqus_identifier %}
