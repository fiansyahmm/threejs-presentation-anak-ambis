# Geometry grouping and merging
## Grouping objects together
In Three.js we can group objects when working with multiple materials. When we create a mesh from a geometry using multiple<br>
materials, Three.js creates a group. Multiple copies of your geometry are added to this group, each with their own specific material. <br>
This group is returned, so it looks like a mesh that uses multiple materials. However, it is a group that contains a number of meshes. <br>

Creating groups is very easy. Every mesh you create can contain child elements, which can
be added using the add function. The effect of adding a child object to a group is that we
can move, scale, rotate, and translate the parent object, and all the child objects will also be
affected. Let's look at an example [01-grouping.html](https://cg2021c.github.io/threejs-presentation-anak-ambis/learning-threejs-master/chapter-08/01-grouping.html). The following screenshot shows 
this example:<br><br>
<img src="https://github.com/cg2021c/threejs-presentation-anak-ambis/blob/main/Geometry%20Grouping%20and%20Merging/image/picture1.jpg?raw=true">
The following code shows how to do this:
```bash
sphere = createMesh(new THREE.SphereGeometry(5, 10, 10));
cube = createMesh(new THREE.BoxGeometry(6, 6, 6));
group = new THREE.Group();
group.add(sphere);
group.add(cube);
scene.add(group);
```
If we look at the controls, we can still move the cube and sphere around and scale and rotate these two objects.
We can also do these things on the group they are in.
If we look at the group menu, we'll see position and scale options

Scale and position are very straightforward. As reminder, when we rotate a group, it doesn't rotate the objects inside it separately; it rotates the entire group around its own center.In this example, we placed an arrow using the THREE.ArrowHelper object at the center of the group to indicate the rotation point:

```bash
var arrow = new THREE.ArrowHelper(new THREE.Vector3(0, 1, 0),
group.position, 10, 0x0000ff);
scene.add(arrow);
Creating and Loading Advance
```

Let's look at an example [01-grouping.html](https://cg2021c.github.io/threejs-presentation-anak-ambis/learning-threejs-master/chapter-08/01-grouping.html). The following screenshot shows 
this example:<br><br>
![screen-gif](https://media.giphy.com/media/hKk9tCVkhF33BZAbZ2/giphy.gif)

When using a group, we can still refer to, modify, and position the individual geometries.
<img src="https://github.com/cg2021c/threejs-presentation-anak-ambis/blob/main/Geometry%20Grouping%20and%20Merging/image/picture2.jpg?raw=true">
