# c2t_lprom

Kolmafia script to fully and automatically use the warbear LP-ROM to make all the recordings. It uses magical sausages as fuel, but can also use mafia's built-in method for MP recovery (untested). Only works for accordion thiefs with their ability to make 20-turn recordings. 10-turn recordings by other classes are not supported with this.

## Installation

It can be installed via the CLI with the following:
* `svn checkout https://github.com/c2talon/c2t_lprom/branches/main/kolmafia/`

### Prerequisites

Make sure to have enough sausages pre-made to recover all the MP needed to cover the costs of the recordings if planning to use sausages, otherwise things may break. Also, wearing gear that increases maximum MP makes things easier and quicker. It takes 6750 MP by default to make the maximimum amount of recordings of all the recordable skills, so plan accordingly. Of course, simply having more than 6750 MP on hand will work as well.

### Usage

First, `import` the function into a script. The following function will be available:

`boolean c2t_lprom(boolean sausageMode)`
* `sausageMode` is optional and determines whether to use magical sausages to recover MP or not. `false` will use mafia's built-in method for MP recovery. Defaults to `true` if omitted
* Returns `true` if it finishes with no critical error. Returns `false` with message if it was unable to finish.

Optionally, it can be called from the CLI simply using its script name, though only with using sausages as fuel, via:
* `c2t_lprom`

