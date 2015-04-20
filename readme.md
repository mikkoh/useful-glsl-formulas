# Useful GLSL Formulas

This repo is a collection of neat formulas I've seen around the Internet. Warning they maybe untested.

Calculate Normals in Fragment Shader:
```glsl
normalize( cross( dFdx( position ), dFdy( position )))
```