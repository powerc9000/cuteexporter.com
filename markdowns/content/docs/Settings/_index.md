---
Title: Project Settings
weight: 200
---

# Project Settings

There are some configurable settings for the app. You can change the settings on the right hand sidebar.
![Location of the settings sidebar in the app](settings-sidebar-location.png)

## Output Directory
This is the folder your final exported assets will output to.

It is saved relative to the folder your project file is saved in.

By default the output directory will be the same folder your project is saved in.

Click on the folder icon to change the output directory.

![Location in the app of the button to change the output directory](output-directory-button.png)

## Output Name
This is the name of the output file your texture and JSON files will be saved as. It will be saved to the output directory.
Changing this value will change the name for the PNG and JSON file.

By default the name of these files is `assets`

## Use Cache

By default Cute Exporter caches individual PNG files into a folder named `cache`. This folder is in the same folder as your project file. If you have many files in your project the cache should increase the speed of re-exports because only the files that have changed since the last export will need to be read.

If you want all your layers as individual PSDs, you can also look into the cache folder for them. They are named by their asset id. i.e `<asset_id>.png`. This will be configurable in the future.

If you don't want to cache any files at all uncheck this box.

If you want a full clean re-export. Delete this folder. It will be remade.

## Trim Alpha

Cute Exporter can trim the extra alpha around your layers. This will lead to your texture atlas being more compact. There are some cases where you may not want this behavior and can uncheck this box.