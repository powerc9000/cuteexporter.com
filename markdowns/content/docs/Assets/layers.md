---
Title: Layers
---

# Layers

Assets can have one or more children (Generically called layers). Layers are what get transformed and output into your texture atlas.

## Layer settings
Layers have a few settings that will affect how they are output.

## Layer Export

When you [export your project]({{<ref "exporting-basics.md">}}), each active layer image is saved to the texture atlas and an entry for that layer is put in the output json file. 

### JSON example

In the output json file there is an array of `assets` each active layer is listed there.

```
{
   "id":"1",
   "name":"folder",
   "parentPath":"raw/icons.psd",
   "width":173,
   "height":128,
   "x":191,
   "y":623,
   "layerPos":{
      "x":0,
      "y":0,
      "width":0,
      "height":0
   },
   "tags":[
      
   ],
   "animationName":"",
   "animationId":0,
   "frameNumber":-1
}
```

You can read about each section in the entry [here.]({{<ref "exporting-basics.md">}}#assets-section)