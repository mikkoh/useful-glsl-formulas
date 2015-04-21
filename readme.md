# Useful WebGL Formulas

This repo is a collection of neat formulas I've seen around the Internet. Warning they maybe untested.

### Get a transformed Normal matrix from a Model matrix
```javascript
var matNormal = glMat3.create();
glMat3.fromMat4(matNormal, model);
glMat3.invert(matNormal, matNormal);
glMat3.transpose(matNormal, matNormal);
```


### Calculate Normals in Fragment Shader:
```glsl
normalize( cross( dFdx( position ), dFdy( position )))
```
