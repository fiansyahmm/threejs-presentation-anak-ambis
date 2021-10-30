# Geometry grouping and merging
## Grouping objects together
In Three.js we can group objects when working with multiple materials. When we create a mesh from a geometry using multiple<br>
materials, Three.js creates a group. Multiple copies of your geometry are added to this group, each with their own specific material. <br>
This group is returned, so it looks like a mesh that uses multiple materials. However, it is a group that contains a number of meshes. <br>

Creating groups is very easy. Every mesh you create can contain child elements, which can
be added using the add function. The effect of adding a child object to a group is that we
can move, scale, rotate, and translate the parent object, and all the child objects will also be
affected. Let's look at an example [01-grouping.html](https://cg2021c.github.io/threejs-presentation-anak-ambis/learning-threejs-master/chapter-08/01-grouping.html). The following screenshot shows 
this example:
