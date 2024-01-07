# Yahtzee.NET Design Document

## Game Engine
Handles the core logic of the game
### Roll Dice
**Dice** need to be kept or rolled.  Max rolls per turn is three.
### Calculate Score
Based on the field selected in the **Scorecard**, score should be calculated, previewed and applied if the user decides.
*Bonus Feature* - provide recommendations to maximize score.
Update total score at the end of the turn.

## Player
Each **Player** will be an object and will have their own **Scorecard**.  When it is their turn, they can use the **Dice**.

## Scorecard
Keeps track of the scores in each category for a player.

## Game Manager
Manages the overall flow of the game.
- Start and end games
- Switch between players when turns end
- Determine Winner

## User Interface
Initially will be ASCII characters in a console window.
