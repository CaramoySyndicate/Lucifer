# Auto Plant Version 0.2

- `moveRange = 5` : Bot skip 5 tile every findPath.
- `moveInterval = 120` : Delay move interval.
  
## Main Config
### Seed
- `seed = 4585` : Seed id to plant.

### Storage Seed
- `storage = {"Storage1|DoorId1","Storage2|DoorId2"}` : Support Multiple World & Multiple Door ID.
  
### Farmlist
- `farmList = {"x","x","x"}` : Write `"farm|doorId"` if using multiple door.
- `doorfarmList = "x"` : id door world farm (ignore this variable if using multiple door).
- `multiplebot = false` : multiple bot at 1 world.
  
  **Multiple Plant :**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/ee53af8a-c14c-4401-b8af-002682f6870e)

  **Single Plant (Planting on 15 tile, more showcase at server) :**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/ca3c492f-67a0-4dff-8669-f4410ac26698)
  
- `worldperbot = 1` : world each bot, auto spread.

  ```
  Example :

  farmList = {"a","b","c","d","e","f","g","h"}
  doorfarmList = "test"
  multiplebot = false
  worldperbot = 2

  Bot 1 planting at world a,b.
  Bot 2 planting at world c,d.
  Bot 3 planting at world e,f.
  Bot 4 planting at world g,h.
  ```
## Features

### Looping mode
- `looping = false` : Set to true if looping take (Nonstop Plant).

### Remove Bot mode
- `removingBot = false` : Set to true if removing bot after all take storage are empty / all drop storage are limit.

### Splice mode
- `splice, seedsplice = false, 1` : set true to splice plant, then write seed splice.
  
## Delay 
### Use Miliseconds
- `delayplant = 120` : Delay on plant.
### Use Seconds
- `delaywarp = 8` : Delay joining world.

- `delayreconnect = 20` : Delay reconnect.

- `delayexecute = 3` : Delay execute each bot.

- `delaylooping = 1` : Delay on Looping take.

### Use Minutes
- `delayidiotserver = 2` : Delay on idiot server (Hard warp).
- `delaymaintenance = 5` : Delay on server maintenance.

## Webhook
**ignore this variable if not using webhook!**
- `webhookstatuslink = "x"` : Write ur webhook link here to info about ur bot status.
  
- `linkbotinfo = "x"` : Webhook link to info about ur bot & storage.
- `messageidbotinfo = {"x","x","x"}` : message id webhook, 1 message per bot
