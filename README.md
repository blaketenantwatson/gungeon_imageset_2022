# gungeon_imageset_2022
Enter the Gungeon Dataset created using Labelbox

## Description
This is a WIP dataset utilizing the popular 2016 video game "[Enter the Gungeon](https://store.steampowered.com/app/311690/Enter_the_Gungeon/)". It currently contains a completely labelled dataset of a frist floor completion, using only the [Marine](https://enterthegungeon.fandom.com/wiki/The_Marine) character and his [base weapon](https://enterthegungeon.fandom.com/wiki/Marine_Sidearm).

## Layout
The provided file layout within this repository is under the 'COCO' dataset configuration, but any format can be generated through [third party websites](https://roboflow.com/convert/labelbox-json-to-coco-json) and the provided labelbox file. The labelbox file contains its own specific format, more documentation for which can be found on [labelboxes website](https://docs.labelbox.com/docs/import-annotations).

## Labels
There are 29 labels, as follows
```
- apprentice_gunjurer
- blobulin_s
- blobuloid_m
- blobulon_l
- blocked_door
- blue_chest
- blue_shotgun_kin
- bookllet_r
- boss_entry
- boss_shades
- boss_smiley
- brown_chest
- bullat
- bullet
- bullet_kin
- dead_apprentice_gunjurer
- dead_blue_shotgun_kin
- dead_boss_shades
- dead_bullet_kin
- dead_red_shotgun_kin
- dead_rubber_kin
- dead_veteran_bullet_kin
- door
- enemy_spawn
- explosive_barrel
- grenat
- health
- hollow_bullet
- hollowpoint
- key
- locked_door
- pinhead
- player
- pressure_plate
- red_shotgun_kin
- rubber_kin
- shopkeeper
- shopkeeper_table
- shotgat
- spirat
- table
- teleporter
- unlocked_door
- veteran_bullet_kin
- wall
- water_pit
```
The descriptions of these enemies can be found on the games [wiki](https://enterthegungeon.fandom.com/wiki/Cult_of_the_Gundead).

## Known Issues
### Underrepresented Classes
There is a noted lack of certain enemy types that can cause false negatives on a number of labels. The following are known to be under represented in the dataset
```
- spirat
- bullat
- grenat
- pinhead
- rubber_kin
- all gunjurer varieties
- key
- health
- armor
- all chests
- all boss entities
```

### Similar Mis-Classifications
There are also a number of enemies that hold a number of similar qualities, and as such can be difficult for models to properly identify. While effort was made to ensure they were not underrepresented within the dataset, they still remain some of the highest error rate labels. More label points are needed to rectify this issue. This issue has occurred on the following labels:
```
- red_shotgun_kin <-> blue_shotgun_kin
- veteran_bullet_kin <-> bullet_kin
- all dead variations of enemies with their living counterparts
```

## Future Plans
For the time being, the only planned expansion to this dataset is the addition of every possible first floor boss. A full dataset for the entirety of the game may be considered at a later point.
