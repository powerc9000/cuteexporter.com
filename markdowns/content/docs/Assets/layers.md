---
Title: Layers
---

# Layers

Assets can have one or more children (Generically called layers). Layers are what get transformed and output into your texture atlas.



## Editing layer data and settings
You can edit the data and settings for your layer by finding it in the layer list of your asset and clicking `edit`

![Screenshot showing the location in a layer where the edit button is located](../edit-layer-link-location.png)

### Layer Active
The active checkbox sets if the layer should be saved to the final output or not. If a layer you expect to show up isn't in your atlas check that the layer is marked as active.

![Screenshot showing where the active checkbox is located in a layer](../edit-layer-active.png)

### Layer Name
You can name your layers whatever you like. This name is exported as `"name"` in the json file.
### Layer Tags
You can give your layers an unlimited number of tags. Tags are a list of string values. 

{{< hint info >}}

You may want to use tags for finding assets in your game engine. You can tag enemies with the tag `enemy` etc.

{{< /hint >}}




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