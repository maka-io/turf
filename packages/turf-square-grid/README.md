# @turf/square-grid

# squareGrid

Takes a bounding box and a cell depth and returns a set of square [polygons](http://geojson.org/geojson-spec.html#polygon) in a grid.

**Parameters**

-   `bbox` **[Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)&lt;[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)>** extent in [minX, minY, maxX, maxY] order
-   `cellSize` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** width of each cell
-   `units` **\[[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)]** used in calculating cellSize, can be degrees, radians, miles, or kilometers (optional, default `kilometers`)

**Examples**

```javascript
var bbox = [-96,31,-84,40];
var cellSize = 10;
var units = 'miles';

var squareGrid = turf.squareGrid(bbox, cellSize, units);

//=squareGrid
```

Returns **[FeatureCollection](http://geojson.org/geojson-spec.html#feature-collection-objects)&lt;[Polygon](http://geojson.org/geojson-spec.html#polygon)>** grid a grid of polygons

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/square-grid
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
