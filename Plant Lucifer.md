# Auto Plant Version 0.2

- `moveRange = 5` : Bot skip 5 tile every findPath.
- `moveInterval = 120` : Delay move interval.
  
## Main Config
### Seed
- `seed = 4585` : Seed id to plant.

### Storage Seed
- `storage = {"Storage1|DoorId1","Storage2|DoorId2"}` : Support Multiple World & Multiple Door ID.
  
### worldFile
- `worldFile = "urworlds.txt"` : **How to make worldList via file?**
  
`Step 1 :` **Open lucifer file, then click right (PC) / hold tap (Smartphone) until this notification appears.**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/89095810-6750-4e60-8d6b-a27376d484f8)

`Step 2 :` **Rename file by urself.**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/9f99db31-e7f0-4324-9ee5-250e6579ff47)

`Step 3 :` **Write ur worldlist on file, WORLD|DOOR**
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/e9a6b755-ea16-477a-b864-febb4a7dddfe)

## Features

### Looping mode
- `looping = false` : Set to true if looping take (Nonstop Plant).

### Remove Bot mode
- `removingBot = false` : Set to true if removing bot after all seed storage are empty.

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
