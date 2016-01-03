leaflet-d3layer
===============

I've started this project to add D3/SVG content to a Leaflet map. There are some amazing samples by 
[Mike Bostock](http://bost.ocks.org/mike/leaflet/) and  [Zev Ross](http://zevross.com/blog/2014/09/30/use-the-amazing-d3-library-to-animate-a-path-on-a-leaflet-map/).
But i had trouble transferring them to my code, as they either have to turn off the zoom-animation or
somehow hijack the leaflet internal SVG _pathRoot object.
I made a layer class that contains its own _pathRoot that is independant from the Leflet SVG-content. 
So i can better control initialization, events an z-Ordering.

I've added both samples to one common demo

http://oliverheilig.github.io/leaflet-d3layer/

Projects where i use this layer:

http://ptv-logistics.github.io/fl-labs/ and http://oliverheilig.github.io/voronoi-territories/

The supported options

* *attribution* - the attribution text for the layer data
* *opacity* - the opacity value between 0.0 and 1.0; default = 1.0
* *zIndex* - z-index of the svg root
* *pane* - the name of the pane where the child div is inserted; default: 'overlayPane' 
* *pointerEvents* - the pointer-events style for the overlayer, default: null
