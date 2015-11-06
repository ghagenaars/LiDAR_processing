# LiDAR_processing
Python files and javascript for pointcloud visualization

The notebooks merges .laz files of the AHN2/AHN3 with aerial photos and outputs a Potree WebGL output. 

The resources folder is used for the Potree Converter and should me in the same folder als the notebooks. It had added features like a watershader, communication with NetCDF files and a different skybox.

The Potree add-on adds a watershader to the point cloud in WebGL. The height of the watershader can be controlled by a slider or using the RWS API. 

For the Potree add-on use the following steps:
Copy folder Watershader, Skybox and Aerial photo to folder the Potree: examples/js
Overwrite viewer.js by viewer.js from this repository
Overwrite build/js/potree.js by build/js/potree.js from this repository for updated pointcloud shader
Merge .las..html files from examples/js.

Wave direction can be controlled in the watershader/WaterShader.js file
