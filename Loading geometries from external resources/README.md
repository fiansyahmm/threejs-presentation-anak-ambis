# Loading geometries from external resources
Three.js can read a number of 3D file formats and import geometries and meshes defined in those files. The following <br>
table shows the file formats that are supported by Three.js:
| Format  | Description |
| ------------- | ------------- |
| JSON | Three.js has its own JSON format that we can use to declaratively define a geometry or a scene. Even though this isn't an official format, it's very easy to use and comes in very handy when you want to reuse complex geometries or scenes.  |
| OBJ or MTL  | OBJ is a simple 3D format first developed by Wavefront Technologies. It's one of the most widely adopted 3D file formats and is used to define the geometry of an object. MTL is a companion format to OBJ. In an MTL file, the material of the objects in an OBJ file is specified. Three.js also has a custom OBJ exporter, called OBJExporter.js.  |
