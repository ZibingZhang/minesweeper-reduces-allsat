# Reduction from Minesweeper to All-Solutions Boolean Satisfiability Problem

__Group members__: Christopher Du, Iris Liu, Iman Moreira, Juniper Parsons, Zibing Zhang

This post will describe the reduction of playing a game of [Minesweeper](https://en.wikipedia.org/wiki/Minesweeper_(video_game)) to solving the all-solution [Boolean satisfiability problem](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem) (AllSAT).

# What is Minesweeper?

Minesweeper is a single-player, puzzle video game in which the player has to "clear" the board without detonating any of the bombs.

This post will focus on the version of Minesweeper that was bundled with Windows 7.
For anyone interested in playing the game, an installation can be found [here](https://minesweepergame.com/download/windows-7-minesweeper.php).
Another version of the game can also be found online [here](https://minesweeper.online/).

## Playing The Game

<!-- ![Before start](assets/before-start.png) -->

![After the first move](assets/post-first-move.png)

The goal of the game is to clear the entire board without detonating any bombs.
After the first move, an area of the board is initially cleared.
Inset tiles have been cleared, while raised tiles have yet to be cleared, or may contain bombs underneath.
The number displayed on a cleared tile indicates the total number of bombs on its adjacent tiles.
Blank tiles are not surrounded by any tiles.

![In progress](assets/in-progress.png)

The player is able to flag tiles they believe to contain a bomb.
The player must methodically click on raised tiles to clear them.

![Completed](assets/completed.png)

The game is over once all tiles that do not contain bombs have been cleared, or once the player clears a tile that contains a bomb.

# What is the Boolean satisfiability problem (SAT)?

For any Boolean formula, the Boolean satisfiability problem is the problem of determining if there exists an assignment of the Boolean variables such that the formula evaluates to TRUE.

# Further Readings

- [Wikipedia Minesweeper Article](https://en.wikipedia.org/wiki/Minesweeper_(video_game))
- [Wikipedia Boolean Satisfiability Problem Article](https://en.wikipedia.org/wiki/Boolean_satisfiability_problem)
