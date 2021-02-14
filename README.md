![b4eec4d093adbe9d8a3cbb40d024836a](https://user-images.githubusercontent.com/72984811/107887784-2e7cf380-6f11-11eb-95f0-16d69e07068d.png)


## 📝 Table of Contents
- [About](#about)
- [Demo](#demo)
- [Install](#Install)
- [How To Play](#play)
- [Built Using](#tech)

## 🧐 About 
It is the well-known game named ```Pacman``` coded in assembly language with x86 instruction set, 8086 version. The game can be played in multiplayer mode on one PC and also on 2 PCs using UART serial communication through the dos emulator ```DOSBox``` with two modes the ```Play``` mode and the ```Chat``` mode in which you can talk with the other player.

The Game has two levels. In level 1 it starts with each player entering with a Pacman from two different sides and The objective of each player is to reach the opposite end before his opponent to be able to win. On his way he will be faced with ghosts moving at the openings of the maze, he must avoid them or he'll die and the other player wins. There will also be powerups like the freeze powerup(if caught by one player it will freeze the other). If the two players collide the game will be over for both. There are five different powerups in total like freeze, start from the beginning, freeze the ghosts, make him Invincible to ghosts or change the other player to a random location. In level 2 the number of ghosts will be increased by 1 and there will be scam powerups that look exactly like the regular ones but here it affects the player who caught it badly (like making him/her go to the beginning and not the opponent).

## 📹 Video

<div name="demo" align="center" width=1189px>
  <p align="center">
    <img width=800px height=410px src="https://user-images.githubusercontent.com/72984811/107890038-3f346600-6f1f-11eb-90be-58193d0eb449.mp4" alt="Video Demo">
    </p>
  </div>  
## 📷 Screenshots

![Screenshot 2021-02-14 234325](https://user-images.githubusercontent.com/72984811/107890008-0c8a6d80-6f1f-11eb-8de1-f033cd7d8890.png)

![Screenshot 2021-02-14 234505](https://user-images.githubusercontent.com/72984811/107890016-1f04a700-6f1f-11eb-9a9f-091aca6f2387.png)
![Screenshot 2021-02-14 234656](https://user-images.githubusercontent.com/72984811/107890019-2330c480-6f1f-11eb-8978-9813b6d2635c.png)


## 🏁 Install
1. Install [DOSBox](https://www.dosbox.com/).
2. Open ```DOSBox Options```.
3. Look for cycles and change it to ```cycles=fixed 1500```

### For the one PC version of the game:

4. Add the following lines to the end of the text file.
```
mount c D:\CMP2023\projects\Pacman
c:
tasm pacman.asm;
tlink pacman.obj;
pacman
```
**Note:** do not forget to replace ```D:\CMP2023\projects\Pacman``` with your local directory. 
### For the two PCs version of the game:
there is a file named ```explanation``` with full insrtuction on how to run the game in this mode
## 💭 How To Play 
For the first player
* ```W``` to move ```UP```
* ```S``` to move ```DOWN```
* ```A``` to move ```LEFT```
* ```D``` to move ```RIGHT```
For the second player
* ```Arrow UP``` to move ```UP```
* ```Arrow DOWN``` to move ```DOWN```
* ```Arrow LEFT``` to move ```LEFT```
* ```Arrow RIGHT``` to move ```RIGHT```
## ⛏️ Built Using 
- [Assembly8086](https://en.wikipedia.org/wiki/X86_assembly_language) - low level programming language.
- [DOSBox](https://www.dosbox.com/) - emulator program.
