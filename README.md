# dynamic-SVG-from-Graphviz
javascript code that can be added to an SVG created by Graphviz to make it dynamic when opening in the browser.

## Features

The following features are currently added:

-Highlighting: when nodes or edges are clicked they are highlighted. this makes is easier to trace certain edges when there are many edges in a diagram

-zoom in or our on cluster: using the + or - button added to every cluster the drwaing is zooming in or out on the cluster.

-visibility switches: CSS classes can be added in grahviz dot to nodes or edges, all classes are listed and by clicking on the class the visibility of all nodes and edges with that class are hidden or shown.


## Usage 🛠️
When you have an svg file generated by graphviz you need to edit the file and

change the svg opening tag by adding  onload="addInteractivity(evt)", giving something like:
```
<svg width="2056pt" height="2297pt" viewBox="0.00 0.00 2056.00 2297.00" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" onload="addInteractivity(evt)">
```


The content of the svg-script file should be added in front of the closing /svg tag.
