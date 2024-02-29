# Auto PNB Version 0.3

## Main Config
- `block = 4584` : Block farmable item id to Pnb.
- `worldpnb = {"world|doorId"}` : All bot will pnb at this variable.
- `posBarisX, posBarisY = 80, 24` : using real growtopia coordinate
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)
- `limitgems = 10000` : limit gems at world pnb, if reached limit, Script terminated.

- `takepickaxe = false` : set true to take pickaxe
- `worldpickaxe = {"world|doorId"}` : ur pickaxe storage

- `withgaut = false` : set true if with gaut.
- `autoRetrieve = false` : set true if auto retrieve, Bot 1 auto retrieve.

## PNB Other Config

- `pnbother = false` : set true to pnbother
- `customWorldPnb = {"worldpnb1","worldpnb2","worldpnb3"}` : world list to pnb
- `doorWorldPnb = "doorPnb"` : door id world pnb
- `worldPerbotPnb = 3` : bot auto arrange

```
Example (Using 3 bots) :

customWorldPnb = {"World1","World2","World3","World4","World5","World6","World7","World8","World9","World10","World11","World12","World13","World14","World15",}
doorWorldPnb = "doorPnb"
worldPerbotPnb = 5

Bot 1 pnb on world1 - world5
Bot 2 pnb on world6 - world10
Bot 3 pnb on world11 - world15

Every pnb or block at backpack are empty, bot taking block then warp to next world

Bot 1 > Pnb on world1 > block at backpack are empty > bot 1 taking blocks > pnb on world2 (Repeat until bot 1 joining on world5)

after joining last world (world5), bot 1 will joining world 1 again, then pnb.

NOTE : Why worldPerbotPnb = 5? cuz u are using 15 worlds and 3 bots, 15 : 3 = 5.
```
- `posBreakX,posBreakY = 80, 24` : using real growtopia coordinate
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

## Storage
### Storage Block

- `storageblock = {"x|x","x|x","x|x"}` : storage block name.

### Storage Seed
- `storageseed = {"x|x","x|x","x|x"}` : storage seed name.
- `amountseed = 100` : amount seed at bot backpack when pnb to storing
- `limitseed = 10000` : limit seed each storage.
  
- `dropseedX, dropseedY = 22, 20` : using real growtopia coordinate
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)

## Pack Config
### Storage Pack
- `storagepack = {"world1|door1","world2|door2","world3|door3"}` : Support Multiple World & Multiple Door ID.
- `limitpack = 10000` : limit pack each storage.
- `droppackX, droppackY = 80, 24` : using real growtopia coordinate.
![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/1e2802e0-daae-4124-b9be-2cf14eea8861)
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
## Features
  
- `autoSkipQuest = false` : set true to skip quest

- `pnbOn25Tile = false` : set true to enable pnb 25 tile (5x5)
 ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/ac42e7cd-586a-4dab-9197-e4b12b91dfef)

- `pnbtile = 5` : custom pnb tile 1 - 5 (ignore if pnbOn25Tile = true)
 ![image](https://github.com/CaramoySyndicate/Lucifer/assets/161619991/9f3b1882-473f-478d-865c-d208cdce52a1)

- `pnbmode = "up"` : choose "up" / "down" / "right" / "left" (ignore if pnbtile = 25)
- `storeseedafterpnb = false` : set true to storing seed after pnb

- `removingbot = false` : set true to remove bot when all block storage are empty / all seed storage are limit.
- `upbackpack = false` : set true to up backpack
- `separated = false` : set true to separating drop
- `sayingrandomwords = false` : set true to enable saying random words before pnb
- `changeSkin = false` : set true to enable change skin

- `whitelistItem = {98,1,1,1,1}` : item list to not trash

## REST
- `botRest = false` : set true to auto rest
- `botRestTime = 600` : bot rest for 10 minutes
- `botRestInterval = 3600`  : bot will rest every 1 hour
- `disconnectOnRest = false` : set true to disconnect every rest

## Delay
### Use Miliseconds
- `delayplace = 110`
- `delaypunch = 185`

### Use Seconds
- `delaywarp = 6`
- `delaydrop = 1`
- `delayretrieve = 8`
- `delayreconnect = 20`
- `delayexecute = 3`
- `delayloginbot = 2` : (delay login for bot switch)

### Use Minutes
- `delayidiotserver = 1` : Delay on hardwarp
- `delaymaintenance = 5` : Delay on maintenance
  
## Webhook
**ignore this variable if not using webhook!**
- `webhookstatuslink = "x"` : Write ur webhook link here to info about ur bot status.
  
- `linkbotinfo = "x"` : Webhook link to info about ur bot & storage.
- `messageidbotinfo = {"x","x","x"}` : message id webhook, 1 message per bot

## Switch account
### Type switch account
- `typeaccount = "normal"` : choose "normal" / "guest" to switch.

### Auto Switch
- `autoSwitch, switchOnLevel = false, 3` : set true to enable auto switch, then write max level bot to switch.

### Letter name guest
- `lettername = 10` : set letter name if use guest.
### Bot per-switch
- `botperswitch = 3` : limit bot perswitch.
- `botSwitch = {
    "user|pass",
    "user|pass",
    "user|pass"
}` : normal ["user|pass"] or guest ["mac|rid"].
```
Example (Using 3 bots) :

botperswitch = 3
botSwitch = {
    "a",
    "b",
    "c",
    "d",
    "e",
    "f",
    "g",
    "h",
    "i"
}

Bot 1 switching on bot "a","b","c".
Bot 2 switching on bot "d","e","f".
Bot 3 switching on bot "g","h","i".
```
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
