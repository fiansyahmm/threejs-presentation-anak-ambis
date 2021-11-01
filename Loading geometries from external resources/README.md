# Loading geometries from external resources
Three.js can read a number of 3D file formats and import geometries and meshes defined in those files. The following <br>
table shows the file formats that are supported by Three.js:
| Format  | Description |
| ------------- | ------------- |
| JSON | Three.js has its own JSON format that we can use to declaratively define a geometry or a scene. Even though this isn't an official format, it's very easy to use and comes in very handy when you want to reuse complex geometries or scenes.  |
| OBJ or MTL  | OBJ is a simple 3D format first developed by **Wavefront Technologies**. It's one of the most widely adopted 3D file formats and is used to define the geometry of an object. MTL is a companion format to OBJ. In an MTL file, the material of the objects in an OBJ file is specified. Three.js also has a custom OBJ exporter, called OBJExporter.js.  |
| Collada | Collada is a format for defining digital assets in an XML-based format. This is also a widely used format that is supported by pretty much all 3D applications and rendering engines. |
| STL | **STL** stands for **STereoLithography** and is widely used for rapid prototyping. For instance, models for 3D printers are often defined as STL files.
Three.js also has a custom STL exporter, called STLExporter.js. |
| CTM | CTM is a file format created by **openCTM**. It's used as a format for storing 3D triangle-based meshes in a compact format. |
| VTK | VTK is the file format defined by **Visualization Toolkit** and is used to specify vertices and faces. There are two formats available: a binary one and a text-based ASCII one. Three.js only supports the ASCII-based format. |
| AWD | AWD is a binary format for 3D scenes and is most often used with the http://away3d.com/ engine. Note that this loader doesn't support compressed AWD files. |
| Assimp | Open asset import library (also called **Assimp**) is a standard way to import various 3D model formats. With this loader, we can import models from a large range of 3D formats that have been converted using **assimp2json**, |
| VRML | **VRML** stands for Virtual Reality Modeling Language**. This is a text-based format that allows to specify 3D objects and worlds. It has been superseded by the X3D file format. Three.js doesn't support loading X3D models, but these models can be easily converted to other formats. |
| Babylon | Babylon is a 3D JavaScript game library. It stores models in its own internal format. |
| PDB | This is a very specialized format, created by **Protein Data Bank**, that is used to specify what proteins look like. Three.js can load and visualize proteins specified in this format. |
| PLY | This format is called the **Polygon** file format. This is most often used to store information from 3D scanners. |
