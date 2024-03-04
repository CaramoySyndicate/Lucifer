# Auto Harvest Version 0.3

- `moveRange = 5` : Bot skip 5 tile every findPath.
- `moveInterval = 120` : Delay move interval.
  
## Main Config
### Block
- `block = 4585` : Block Id Farmable to harvest.

### worldFile
- `worldFile = "urworlds.txt"` : **How to make worldList via file?**
  
`Step 1 :` **Open lucifer file, then click right (PC) / hold tap (Smartphone) until this notification appears.**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/89095810-6750-4e60-8d6b-a27376d484f8)

`Step 2 :` **Rename file by urself.**
  ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/9f99db31-e7f0-4324-9ee5-250e6579ff47)

`Step 3 :` **Write ur worldlist on file, WORLD|DOOR**
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/e9a6b755-ea16-477a-b864-febb4a7dddfe)

 ## Storage
 ### Storage Block
- `storageblock = {"world1|door1","world2|door2","world3|door3"}` : Support Multiple World & Multiple Door ID.
- `limitblock = 10000` : limit block each storage.
- `amountblock = 180` : limit block when harvest to storing.
- `dropblockX, dropblockY = 80, 24` : using real growtopia coordinate.
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

### Storage Seed
- `storageseed = {"world1|door1","world2|door2","world3|door3"}` : Support Multiple World & Multiple Door ID.
- `limitseed = 10000` : limit seed each storage.
- `amountseed = 150` : limit seed when harvest to storing.
- `dropseedX, dropseedY = 80, 24` : using real growtopia coordinate.
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

## Pack Config
### Custom buying pack
- `buypack = false` : set true to buying pack.
- `packList = {1,1,1,1}` : item id pack list.
- `debug = "debug_pack"` : debug pack.
- `mingems = 1` : minimum gems to buying pack.
- `pricepack = 1` : price pack at store.
  ```
  Example buying Master Surgeon's Tool Bag :
  
  buypack = false
  packList = {1270, 4316, 4310, 1258, 4312, 4318, 4308, 1260, 1268, 4314, 1264, 1266, 1262, 4296}
  debug = "surg_value_pack" : debug pack.
  mingems = 45500 : minimum gems to buying pack.
  pricepack = 45000 : price pack at store.
  ```
### Storage Pack
- `storagepack = {"x|x","x|x","x|x"}` : Support Multiple World & Multiple Door ID.
- `limitpack = 10000` : limit pack each storage
- `droppackX, droppackY = 80, 24` : using real growtopia coordinate
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)
## Special event

- `eventList = {1,2,3,4,5}` : item id special event
- `wearingItemSupport = false` : set true to wear item, like using magnifience at harvest festival
- `idItemSupport = 1` : item id to wear
- `amountEvent = 1` : limit item event when harvest to storing.
- `keepItemSupport = 1` : after take & wear special event item like magnifience, The bot drops items and leaves an amount according to this variable.
- `worldwearitem = {"world|door"}` : World take special event item to wear

- `storageevent = {"world1|door1","world2|door2","world3|door3"}` : Support Multiple World & Multiple Door ID.
- `limitevent = 10000` : limit event each storage.
- `dropeventX, dropeventY  = 80, 24` : using real growtopia coordinate.
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

## Features
- `recycle = false` : set true to recycle block.
- `separated = false` : set true to separating drop.
- `ignoregems = false` : set true to ignoring gems.
- `removingbot = false` : set true to removing bot after finished all farm / all storage are limit.
- `upbackpack = false` : set true to up backpack.
- `range = 5` : custom range to collect when harvest.

- `clearhistory = false` : set true to joining random world after storing items.
- `worldclearhistory = {"x","x","x"}` : world to join after storing items.
  
## Delay 
### Use Miliseconds
- `delayharvest = 120`
### Use Seconds
- `delaydrop = 1`
- `delaywarp = 8`
- `delayreconnect = 20`
- `delayexecute = 3`
- `delayloginbot = 2` : delay login bot when switch accs
### Use Minutes
- `delayidiotserver = 2` : Delay on hard warp
- `delaymaintenance = 5` : Delay on maintenance

## Webhook
**ignore this variable if not using webhook!**
- `webhookstatuslink = "x"` : Write ur webhook link here to info about ur bot status.
  
- `linkbotinfo = "x"` : Webhook link to info about ur bot & storage.
- `messageidbotinfo = {"x","x","x"}` : message id webhook, 1 message per bot

## Switch account
### Auto Switch
- `autoSwitch, switchOnLevel = false, 3` : set true to enable auto switch, then write max level bot to switch.
### Type switch account
- `typeaccount = "normal"` : choose "normal" / "guest" to switch.
### Letter name guest
- `lettername = 10` : set letter name if use guest.
- `switchFile = "switch.txt"` : same as worldFile 
### Proxy Config

- `withproxy, botperproxy = false, 1` : set true to using proxy, then setting limit bot per proxy/
- `proxyList = {
    "ip:port:user:pass",
    "ip:port:user:pass",
    "ip:port:user:pass"
}` : Proxy list
```
  Example (Using 15 bots switch and 5 bot per proxy) :

  withproxy, botperproxy = true, 5
  proxyList = {
    "123.45.678:1000:caramoy:caramoy",
    "123.45.678:1001:caramoy:caramoy",
    "123.45.678:1002:caramoy:caramoy",
  }

  Bot 1 - 5 : "123.45.678:1000:caramoy:caramoy"
  Bot 6 - 10 : "123.45.678:1001:caramoy:caramoy"
  Bot 11 - 15 : "123.45.678:1002:caramoy:caramoy"
```
