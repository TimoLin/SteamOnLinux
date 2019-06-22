Lutris Install The Witcher3: Wild Hunt - Game of The Year Edition
==========
In steam, it's very easy to install The Witcher 3-GOTY through Steam Play and Proton.  
How ever if you have the GOG version, it's not very easy to install as in Steam.   
Luckily we have an open source solution: [lutris](https://github.com/lutris/lutris).  

A user shared his install script at [Install TW3-GOTY](https://github.com/lutris/lutris). But when using it, the downloading procedure alwasy stops at somewhere when downloading The Witcher 3 installer files since it's too big (4G files). And also there is an issue __"if u dont download but select the setup the installer never finish"__.  
So I found another way to mannually download the files from GOG and copy them to the lutris cache folder to solve this issue.

Under Ubuntu 18.04.2, NVIDIA drivers 390.116.

## Firstly, click preference setting of lutris:  
![](https://user-images.githubusercontent.com/7792396/59961926-86334380-9511-11e9-978b-c31378e2234a.png)   
## Secondly, set the "Cache path"  to  a folder in your local computer, here we use `/home/myubuntu/game/cache` as an example.  
![](https://user-images.githubusercontent.com/7792396/59961942-90edd880-9511-11e9-852c-0aef3b13d06d.png)  
## Thirdly, try to install The Witcher 3 GOTY through the script, you will find a folder is created in the folder your set: `/home/myubuntu/game/cache/the-witcher-3-wild-hunt-game-of-the-year-edition`,  cancel the installation.  
![](https://user-images.githubusercontent.com/7792396/59962058-eb3b6900-9512-11e9-98f1-75d024496675.png)  

## Finally, copy your downloaded TW3-GOTY installergg files to the `gog` folder and then install the game through the script.
`/home/myubuntu/game/cache/the-witcher-3-wild-hunt-game-of-the-year-edition/gog/`.  

## Enjoy it.  

It took me less than an hour to install it and the game opens successfully but ~~i don't have time to test playing the game right now~~.  

## Controller support
Test the game tonight. It runs smoothly. For thoes who use a contorler to play, [this thread](https://forums.lutris.net/t/controller-joypad-setup-in-lutris-with-wine-steam/1204/2) may help you.  
For me I use BETOP BTP-2126E controller and use the same setting as the thread.  
![](https://user-images.githubusercontent.com/7792396/59964685-606c6580-9536-11e9-94a0-66e5e5f15f3b.png)
