# The Waterfinder

A Minesweeper-style game built for charity: water. Dig down through soil,
avoid contaminated water, and reach the clean water below. Four difficulty
levels, scored on time.

**[Play it →](https://emcuberos1.github.io/waterfinder/)**

## Features

- Four difficulty levels that change board size, obstacle density and pace
- Timed play with a best-time record rather than a points score
- Milestone messages at key moments — breaking through topsoil, reaching
  halfway, uncovering clean water
- Sound effects for digging, winning and losing
- A mobile layout with fewer columns and more rows, so the same puzzle fits a
  narrow screen
- charity: water brand fonts and colors, with links to their site and
  donation page

## Built with

HTML, CSS and vanilla JavaScript. No framework.

## A note on board generation

Early versions sometimes produced boards where the player had no way to deduce
the next safe tile and simply had to guess. The cause turned out to be board
generation rather than how much information was being shown. The game now
generates a board, solves it against itself to confirm it can be won without
guessing, and discards any board that fails that test.

## Design approach

The goal was not a game with a charity's logo on it, but one that puts the
player in charity: water's position. The mechanic comes from how they actually
drill wells: water near the surface isn't safe to drink, so you have to get
past it to reach what is.
