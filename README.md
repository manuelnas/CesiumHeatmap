# CesiumHeatmap
A library to add heatmaps (using heatmap.js) to the Cesium framework.

**CesiumHeatmap.js**

This is a library that uses either a Entity.Rectangle or the SingleTileImageryProvider to add the heatmap to the globe. To use this on your page do the following:

- Import the CesiumHeatmap.js file into your page using the <script> tag. This file includes heatmap.js.
- Initialize a CesiumHeatmap instance using the `CesiumHeatmap.create()` call. See the function in the code for more information on parameters.
- Add the data points to the CesiumHeatmap instance using the `instance.setData()` or more likely `instance.setWGS84Data()`. See the functions in the code for more information on the parameters.
- After new data is added to the CesiumHeatmap instance it will automatically show/update the layer.
