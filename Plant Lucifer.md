# Auto Plant Version 0.2


## Main Config
### Seed
- `seed = 4585` : Seed it to plant.

### Storage Seed
- `storage = {"Storage1|DoorId1","Storage2|DoorId2"}` : Support Multiple World & Multiple Door ID.
  
### Farmlist
- `storageTake = {"Storage1|DoorId1","Storage2|DoorId2"}` : Support Multiple World & Multiple Door ID.
- `limit = 10000` : Limit items amount each world.
- `posX, posY = 80,24` : Using real growtopia coordinate.

![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

## Features
### Looping mode
- `looping = false` : Set to true if looping take (Nonstop moving).
### Separated mode
- `separated = false` : Set to true if dropping items each tile.
  
### Only 1 item id :

![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/d52f2d44-7e80-41cb-9468-42c08cf6b6e2)

### Items Id more than 1 :

![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/c80c33c6-ac77-4bcc-81c4-22ca70077a90)

### Remove Bot mode
- `removingBot = false` : Set to true if removing bot after all take storage are empty / all drop storage are limit.

## Delay 
### Use Seconds 
- `delaywarp = 5` : Delay on joining world.
- `delaydrop = 2` : Delay on dropping Item Id.
- `delayexecute = 5` : Delay execute each bot.
- `delayreconnect = 10` : Delay on reconnect.
- `delaylooping = 1` : Delay on Looping take.
### Use Minutes
- `delayidiotserver = 2` : Delay on idiot server (Hard warp).
- `delaymaintenance = 5` : Delay on server maintenance.

## Webhook
**ignore this variable if not using webhook!**
- `webhookstatuslink = "x"` : Write ur webhook link here to info about ur bot status.
- `linkbotinfo = "x"` : Webhook link to info about ur storage.
- `messageidbotinfo = "x"` : Message id webhook, Check server if u cant get message Id.
