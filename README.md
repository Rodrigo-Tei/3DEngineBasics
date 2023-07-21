# 3DRenderBasics
Study project of the basics of 3D rendering. This study was based on javidx9's project.

## Description

This project renders a cube spinning. The implementation also has a camera, that can be controlled with the standar movimentation controls (WSAD) and the keyborad arrows (&larr; &rarr;).

## The Cube

The cube is constructed by a mesh of triangles. Each face of the cube has two triangles and each triangle is a set of 3 coordinates.

The rotation is calculated using the [rotations matrix](https://en.wikipedia.org/wiki/Rotation_matrix#:~:text=in%20its%20center.-,Basic%20rotations,-%5Bedit%5D).

The illumination is set on origin (0,0,0), pointing to the cube. Each face has a color, that is calculated using the normal vector of each face and the direction of the light.

The camera is calculated by the rotation of the space, and then setting each point of the rotated cube.

## Render working

<img src='doc/cube.gif'>

