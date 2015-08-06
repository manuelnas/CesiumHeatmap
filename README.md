# CesiumHeatmap
A library to add heatmaps (using heatmap.js and `Cesium.Entity.Rectangle` or `Cesium.SingleTileImageryProvider`) to the Cesium framework.

To use this on your page do the following:

- Import the CesiumHeatmap.js file into your page using the `<script>` tag. This file includes heatmap.js.
- Initialize a CesiumHeatmap instance using the `CesiumHeatmap.create()` call. See the function in the code for more information on parameters.
- Add the data points to the CesiumHeatmap instance using the `instance.setData()` or more likely `instance.setWGS84Data()`. See the functions in the code for more information on the parameters.
- After new data is added to the CesiumHeatmap instance it will automatically show/update the layer.

# HeatmapImageryProvider.js
A library to add heatmaps (using heatmap.js) to the Cesium framework using a custom `Cesium.ImageryProvider`.

To use this on your page do the following:

- Follow the steps in the comment on the first few lines of the file to add the class to Cesium.
- Create a HeatmapImageryProvider instance like so: `new Cesium.HeatmapImageryProvider()`. See the function in the code for more information on the parameters.
- Add the instance to the `widget.scene.imageryLayers` list like so: `var layer = widget.scene.imageryLayers.addImageryProvider(instance)`. After this you can use layer like any other layer in Cesium.
