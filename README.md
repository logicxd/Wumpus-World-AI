# Wumpus World AI
2nd highest scoring AI bot for a class tournament that aims to find the gold and escape the Wumpus World with the best possible score.

![SamplePlay](https://user-images.githubusercontent.com/12219300/43773157-a362492e-99f9-11e8-8836-15771b6dfd99.gif)

Map Info:
* B = Breeze
* P = Pit
* W = Wumpus
* G = Gold
* @ = Player
* . = Tile

## Scoring

The performance measure of an agent is an integer score calculated based on the following:
* Start at 0 points
* -1 point for each action taken
* -10 for using the arrow (additional to the -1 point)
* -1000 points for falling into a pit or being eaten by the wumpus +1000 for climbing out of the cave with the gold

The game ends either when the agent dies, when the agent climbs out of the cave, or when the agent’s score goes below -1000.

Score of **283.87** was averaged over 10,000 randomly generated worlds that are 4x4 to 7x7, with each square having a 20% chance of pit appearing.
