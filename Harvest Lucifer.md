# Auto Harvest Version 0.2

- `moveRange = 5` : Bot skip 5 tile every findPath.
- `moveInterval = 120` : Delay move interval.
  
## Main Config
### Block
- `block = 4585` : Block Id Farmable to harvest.

### Farmlist
- `farmList = {"x","x","x"}` : Write `"farm|doorId"` if using multiple door.
- `doorfarmList = "x"` : id door world farm (ignore this variable if using multiple door).
- `multiplebot = false` : multiple bot at 1 world.
  
  **Multiple Harvest :**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/76a9c182-e46f-40b9-90eb-0007a14c4383)


  **Single Harvest (Harvesting on 15 tile, more showcase at server) :**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/49a16fa6-5be8-4f77-b9fb-651ba932e03b)

  
- `worldperbot = 1` : world each bot, auto spread.

  ```
  Example :

  farmList = {"a","b","c","d","e","f","g","h"}
  doorfarmList = "test"
  multiplebot = false
  worldperbot = 2

  Bot 1 harvesting at world a,b.
  Bot 2 harvesting at world c,d.
  Bot 3 harvesting at world e,f.
  Bot 4 harvesting at world g,h.
  ```
 ## Storage Block & Seed 
