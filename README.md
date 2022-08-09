# Real Estate Game Lite
A backend version of the boardgame classic using Python.
<br></br>

## Table of Contents
- [Overview](#overview)
- [Setup](#setup)


## Overview
Don't have five hours to play the classic Monopoly?  This "lite" version of the famous real estate board game helps simulate the original.

Players start at "GO" and then take turns rolling a single six-sided die, and moving around the board. The spaces are created as a linked list, and players will move around the board circularly. The amount of money each player receives at the start of the game is determined at game setup. Each space on the board may be purchased except for "GO". Once a space is owned, the owner charges rent to other players who land on the space. When a player runs out of money, that player becomes inactive in the game, and can no longer move. End game occurs when only one player has a positive account balance.


## Setup

The project provides the backend functionality of a condensed version of your favorite real estate board game.  Below is a mock setup to run the game:
```
BoardGame = RealEstateGame()

rents = [50, 50, 50, 100, 100, 100, 200, 200, 200, 250, 250, 250, 300, 300, 300, 325, 325, 325, 350, 350, 350, 375, 375, 500, 500]

BoardGame.create_player("Ringo", 1000)
BoardGame.create_player("McCartney", 1000)
BoardGame.create_player("Lennon", 1000)
BoardGame.create_player("George", 1000)

BoardGame.move_player("McCartney", 4)
BoardGame.buy_space("McCartney")
```
