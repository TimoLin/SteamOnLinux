SteamOnLinux
=======================
Playing Steam games on Linux is awesome.  

## [1 Sid Meier's Civilization V](https://store.steampowered.com/app/8930/Sid_Meiers_Civilization_V/)  
### 1.1 Civilization V  crashs randomly on Linux.  
[Check this solution at reddit](https://www.reddit.com/r/civ5/comments/5z77jr/game_crashes_randomly_on_linux_amd_ryzen/)  
```shell
cd ~/.local/share/Aspyr/Sid\ Meier\'s\ Civilization\ 5  
vim config.ini  
```
Change `MaxSimultaneousThreads=8` to `MaxSimultaneousThreads=16`  

### 1.2 Chinese for civ5 linux  
[liujingchen/civ5cn-linux](https://github.com/liujingchen/civ5cn-linux). Follow the instruction in Readme.md   

### 1.3 Ingame editor mod  
[boekkooi/CIV5_IGE_LINUX](https://github.com/boekkooi/CIV5_IGE_LINUX)  

## [2 Left 4 dead 2](https://store.steampowered.com/app/550/Left_4_Dead_2/)
### 2.1 Chines font for L4D2 Linux
Install this font:  
```shell
sudo apt-get install fonts-wqy-zenhei
```
[Check this solution](https://github.com/ValveSoftware/steam-for-linux/issues/3255)

## 3 Steam play don't show
[Check this](https://steamcommunity.com/app/221410/discussions/8/1736589519990509315/) 
__Warn: This solution will remove all your downloaded games! Use this at your own consideration.__
Maybe it's because your steam linux version is too old.  
You can try to remove steam dir and reopen steam to let steam update itself.  
```shell  
rm ~/.local/share/steam
rm ~/.steam
```  

## 4 Proton for Non-Steam games
1. Right click the added non-steam game in your Library and click on `Properties`    
2. Check option `Force the use of a specific Steam Play compatibility tool`  
3. Enjoy it  

## 5 Pillars of Eternity
### 5.1 Mouse doesn't work under dual monitor
Unplug one monitor, start game and mouse works. Then uncheck **Fullscreen** to avoid problems in dual monitor situations. Plug the other monitor back and you can play PoE under the window mode.
### 5.2 Chinese language display problem
If you use Chinese (Simplified or Traditional), there may be a problem displaying Chinese in the game, missing some text or characters for example. This is due to Microsoft Yahei(微软雅黑) font is not installed in your system.
Here is a brief instruction to install Yahei font:  
1. Get `msyh.ttc`, `msyhl.ttc` and `msyhbd.ttc` from Windows or internet.
2. `cd /usr/share/fonts`
3. `sudo mkdir WindowsFonts`
4. `sudo cp YourFontPath/msyh*.ttc WindowsFonts/`
5. `sudo chmod 755 /usr/share/fonts/WindowsFonts/*`
6. `fc-cache`
Start game and check if Chinese displays crectly.  
