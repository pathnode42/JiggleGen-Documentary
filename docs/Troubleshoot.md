# Troubleshoot

Most problems that you might encounter are connected to the 'Surface Deform' Modifier. The problem isn't always very clear and easy to solve. Personally always found a solution with the error Code + google.

| Problem | Solution |
|---------|---------|
| Add-on does not appear in Blender | Go to **Preferences → Add-ons**, search for "JiggleGen", and enable it |
| Target-Mesh is not following the ProxyMesh | Go to Target Mesh -> Review the 'Surface Deform' Modifier |
| 'Surface Deform' Modifier: Target has Edges with more than two Polygons | Check the generated Geometry for multiple faces. Usually the boundaries of the mesh creates problems. Change the VertexGroup Selection. |
| 'Surface Deform' Modifier: Target contains concave polygons | Tirangulate Modifier on ProxyMesh usualy solves this. |
| Presets are not showing | Refresh Preset Panel |
||Make sure Presets are installed in the right directory. Check for Presets > [Installation](/docs/Installation.md) |
