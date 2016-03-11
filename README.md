# cs56-games-battleship

This is an extended version of the game Battleship. 

project history
===============
```
 W14 | andrewberls 5pm | OliverHKU  | Battleship game
```

* Original developer description - the Milton Bradley board game that has won the hearts of children for over four decades. It will be single-player (vs. computer) and will have various difficulty settings (easy, normal, hard).  You can also host/join games and play against your friends online WITH THE POWER OF JAVA NETWORKING!

* Current version: 2.2
* Previous versions:
	* version 1: See "Original developer description" (see figure 0)
	* version 2.0: New feature added. Player can customize ship sizes in the "against computer" mode through a new window.(see figure 1) Illegal ship sizes will be reported to the player. (see figure 2)
	* version 2.1: New feature added. There will be a hit count under the game board indicating how many pixels on the opponent's ship has the player already hit. (see figure 3)
	* <b>version 2.1.1</b>: Bug fix on checking ship sizes validity. In version 2.0, if user input is not a number, program will terminate. Now fixed. (see figure 4)
    * <b>version 2.2</b>: Game now has replay functionality, ship color selection, harder computer difficulty, and sound effects.

* Game description - this Battleship game has 3 modes for user to choose from: hosting a game, joining a game, and playing against a computer. (see figure 5)
	
	* Hosting a game: User's IP address will be displayed, and user shall wait for someone else to join his game.
	* Joining a game: User shall be told the host's IP address, and input the IP address to join a game.
	* Playing with a computer:
		* User can customize ship sizes from 2 to 9. [since version 2.0]
		* There are 3 difficulty levels in the game, EASY, MEDIUM and HARD.


* For future developers:
	* There are 5 classes included in the package. BattleshipController is the controller of the game including the main method to be run. BattleshipGUI is for setting up the GUI. The other three classes are player classes, representing individual players. I recommend that you start with looking at BattleshipGUI.java.

* <b>W16 final remarks</b>
    * This game is of the model-view-controller design pattern
    * <b>Note about sound effects:</b> You must be on a CSIL machine or your own personal machine to get sound effects to work, you can't play them through ssh'ing. 
    * The sound effects are currently set to the lower bitrate sound effects so that they play better on CSIL, but there are higher quality sound effects that sound much better. To change to the higher bitrate sfx, edit BattleshipGUI.java and find the URL initializations and change all of the file extensions from .aiff to .wav.
    * When running sound effects on a CSIL machine, after the sounds haved played ~30 times the system can't handle them anymore and the sound effects will stop working.
    * Test cases are very underdeveloped for this project, there's a lot of room for work there.

	* Suggested improvement to be made:
        * Make the game adaptable to the Internet. Currently the game can only be played within the same network, is it possible that it be played by 2 players 5000 miles from each other?
        * Somehow get the sound effects to not crash when playing them on a CSIL machine
        * Add options to go back to previous windows when setting up a game
        * Rework the GUI to use actual graphics instead of colored squares


The code can also be found at these links

- [Archive page](https://foo.cs.ucsb.edu/cs56/issues/0000501/)


Figure 0
![](http://i.imgur.com/AUr93FG.png)


Figure 1
![](http://i.imgur.com/Pc82RXX.png)


Figure 2
![](http://i.imgur.com/PnBQ9Lu.png)


Figure 3
![](http://i.imgur.com/1iNCHmp.png)


Figure 4
![](http://i.imgur.com/djezD7F.png)


Figure 5
![](http://i.imgur.com/svm5tkM.png)


Figure 6
![](http://i.imgur.com/tFAAbk8.png)


<b>FAQ</b>

1. How to run the program?
	* In Unix command line or MacOS terminal, simply type ant run.
	* In Windows or Android machines with Java installed, run the .jar file directly.
2. How come sound effects aren't playing?
    * Sound effects won't play if you're trying to run the program over ssh
    * You must run the program on a physical CSIL machine or run the .jar file locally on your own machine
