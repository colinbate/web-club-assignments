# Battleship

## Background

Up to this point, the exercises have been useful and hopefully somewhat interesting, but not particularly fun and exciting. I'm hoping this one will be more so, if nothing else something you may be interested in showing your friends and family.

We are going to make a game. In particular, a version of the classic board game: Battleship. If you aren't familiar with it, I'll explain what we specifically want below. However, in a nutshell it is a two player, turn-based game whereby your goal is to guess the position of and sink your opponent's fleet of ships.

## Stack Requirements

Before I just suggested that you use something new to you to build your app. That is something I'm always going to advocate you do. Instead, I'm going to suggest the additional restriction of not using any framework or libraries from any of the "big players". So no Google, no Facebook, no Microsoft, no Yahoo, no Twitter.

So on the JS framework side, you may want to try:

* [Mithril](http://mithril.js.org/)
* [Cycle.js](http://cycle.js.org/)
* [Riot.js](http://riotjs.com/)

And on the CSS side you can consider:

* [UI Kit](http://getuikit.com/)
* [Semantic UI](http://semantic-ui.com/)

Also, and this is particularly important if you haven't done so already, please try to use ES2015 syntax.

## Game Requirements

There are actually two versions of this game that could be built. One is the single player version where you play against the "computer". The other version is two player and you play against another human player. This version has two different sub-versions, one which is pass-and-play, mostly suited to mobile devices, and the other over web sockets with another browser or machine.

I'm not going to require a specific version, as each offers different challenges. Ultimately a good solution should offer all three variations.

Specific things that should be present:

* Application should initialize to a "Start Game" screen with some sort of play button, potentially allowing some game customizations.
* There should be two grids of 10x10 squares displayed.
* The player should be allowed to place her ships on one of the grids.
* The game should decide randomly who goes first.
* On your turn, you select one of the squares on the enemy grid to attack.
  * If your attack hits an opponent's ship, notify both players and mark a red indicator on the enemy gird and on the hit ship.
  * If the attack misses, mark a white indicator on the enemy grid.
  * Once a square is attacked, it should not be available to attack again.
* If a ship is hit on each space, announce to both players that the ship was sunk.
* Once a player loses all of their ships, the game is over and the other player is the winner.

You shouldn't need to use canvas for this game, but you are welcome to use it if you'd like. I would recommend some use of animation and/or audio to add some realism to the game, but these things are secondary to the main gameplay.

## Other Optional Enhancements

Obviously there are many more enhancements which could be made in the area of graphics and audio, as well as game play. Things like recording high scores, in game chat, etc are all possible. Feel free to take this wherever you see fit.