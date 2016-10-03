3D Models for SparkFun Products!
----------------

This is a repository of basic geometry and source CAD (if we have them) files for 3D models that appear on our website. Models are stored in real world (1x) scale. STL units are millimeters.

_If you are using [eagleUp](https://eagleup.wordpress.com/) be sure to only export ```Place``` layers_

## Directory Structure

Folders and file names must only use a-z, - and _

#### Product geometry model structure:
```
products/{product_id}/{rev_if_applicable}/{file_type}/

Ex:
products/12099/iges/12099.iges
products/12099/step/12099.step
products/12099/stl/12099.stl

If there were any revisions for this product_id:
products/11113/rev_1.0/stl/11113.stl
products/11113/rev_1.1/stl/11113.stl
```

#### Source model structure:
```
products/{product_id}/{rev_if_applicable}/source_{software}/

Ex:
products/11763/source_solidworks/model.sldprt

If there were any revisions for this product_id:
products/11763/rev_1.0/source_solidworks/11763.sldprt
products/11763/rev_1.1/source_solidworks/11763.sldprt

```

#### Product display structure:
We can display any combination of stl or json with textures
```
products/{product_id}/display/modela.stl

Ex:
products/8601/display/8601a.stl
products/8601/display/8601b.json
products/8601/display/8601b_texture.png
```
Hex for Lilypad 0x8000FF (purple)

## Blender Common Display Materials

_Use the io_three blender addon in the https://github.com/mrdoob/three.js repository to export textured display models for our site_

_Be sure to set your scene's display device to none before export to prevent colors from being gamma corrected. Or use the startup file in this repo._

For composite display models, commit the blender file with separate objects for easy tweaking in the future. Combine the geometry before exporting to json.

#### Copper
```
Diffuse:  #DF8D38 Intensity: 0.8
Specular: #FFB730 Intensity: 0.5
Hardness: 100
```

#### Leads
```
Diffuse:  #FFFFFF Intensity: 0.8
Specular: #E6E6E6 Intensity: 0.5
Hardness: 100
```

#### Black plastic (Headers, specifically)
```
Diffuse:  #000000 Intensity: 0.8
Specular: #A5A5A5 Intensity: 0.5
Hardness: 50
```

#### Black chip
```
Diffuse:  #000000 Intensity: 1.0
Specular: #222222 Intensity: 0.5
Hardness: 50
```

#### SFE Red Silk
_Solid Material_
```
Diffuse:  #98041C Intensity: 1.0
Specular: #98041C Intensity: 0.5
Hardness: 50
```
_Textured Material_)(red)
```
Diffuse:  #FF2835 Intensity: 0.8
Specular: #98041C Intensity: 0.5
Hardness: 50
```
#### Blue plastic (Screw Terminals)
```
Diffuse:  #0000FF Intensity: 0.8
Specular: #0000A5 Intensity: 0.5
Hardness: 50
```
#### Blue PCB (Arduino)
```
Diffuse:  #0C457C Intensity: 0.8
Specular: #0F4E7A Intensity: 0.5
Hardness: 50
```

#### White Plastic
```
Diffuse:  #FFFFFF Intensity: 0.8
Specular: #E2E2E2 Intensity: 0.8
Hardness: 25
```

#### Grey Plastic
````
Diffuse:  #8A8A8A Intensity: 1.0
Specular: #FFFFFF Intensity: 0.25
Hardness: 50
```

#### Yellow Plastic (Li-ion Battery)
````
Diffuse:  #CC9D00 Intensity: 0.8
Specular: #FFD700 Intensity: 0.5
Hardness: 50
```

#### SMD Resistor Brown
```
Diffuse:  #8F5A24 Intensity: 0.8
Specular: #FFB730 Intensity: 0.5
Hardness: 100
```

#### Component Black
```
Diffuse:  #111111 Intensity: 0.8
Specular: #222222 Intensity: 0.5
Hardness: 100
```

#### Green Protoboard
```
Diffuse:  #00703D Intensity: 0.8
Specular: #0A5D19 Intensity: 0.5
Hardness: 100
```

#### Brown Resistor
```
Diffuse:  #835715 Intensity: 0.8
Specular: #AA630Ab Intensity: 0.5
Hardness: 100
```

#### Brown Resistor
```
Diffuse:  #835715 Intensity: 0.8
Specular: #AA630Ab Intensity: 0.5
Hardness: 100
```