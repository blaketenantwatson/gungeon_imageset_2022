# gungeon_imageset_2022
Enter the Gungeon Dataset created using Labelbox

# Description
This is a WIP dataset utilizing the popular 2016 video game "Enter the Gungeon". It currently contains a completely labelled dataset of a frist floor completion, using only the marine character and his base weapon.

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
The descriptions of these enemies can be found on the games wiki.

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
There are also a number of enemies that hold extremely similar 
