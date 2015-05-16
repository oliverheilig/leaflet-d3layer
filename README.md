# leaflet-d3layer
A less hackish way to use D3 with Leaflet

I've started this project to add D3/SVG content to a Leaflet map. There are some amazing samples by 
[Mike Bostock](http://bost.ocks.org/mike/leaflet/) and  [Zev Ross](http://zevross.com/blog/2014/09/30/use-the-amazing-d3-library-to-animate-a-path-on-a-leaflet-map/).
But i had trouble transferring them to my code, as they either have to turn off the zoom-animation or
somehow hijack the leaflet internal SVG _pathRoot object.
So i made a layer class that contains it's own _pathRoot that is independant from the Leflet SVG-content. 

I've added both samples to one common demo

http://oliverheilig.github.io/leaflet-d3layer/

I'm using this approach at this code sample for my company's routing services

http://ptv-logistics.github.io/fl-labs/

Hope i can extend this class when i'm more familiar with D3/SVG.
