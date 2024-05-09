# v1.2.6
- fix interaction with slope stacks
- make the wave snapping to blocks visible, drawing a vertical line
- copy player 2 data to player 1 if in dual mode and player 2 touches a single portal
- make error margin inversely proportional to delta time (less likely to double up a point with Click Between Frames)

# v1.2.5
- fix interaction with orbs
- fix interaction with spider pads

# v1.2.4
- remove the smoothening from the previous update, as Click Between Frames got fixed in v1.0.7

# v1.2.3

- add some smoothening to fix duplicating points with Click Between Frames
- fix wave trail not being visible on Android

# v1.2.2

- fix crashes on some levels which teleport you instantly as soon as the level starts
- make the wave trail correct on levels which teleport you instantly as soon as the level starts
- fix the wave trail looking wrong on levels with a start position

# v1.2.1

- add extra checks for whether you are in-game

# v1.2.0

- fix behavior with spider orbs
- fix the wave trail looking bad if you have Click Between Frames installed
- fix practice mode bug when the player is hidden
- try to make wave trail more accurate when colliding with blocks

# v1.1.7

- fix teleport portal regression

# v1.1.6

- fix the trail showing up in the editor when the player reverses direction
- fix the trail not showing as soon as you switch direction
- refactor code and account for cumulative error on smooth transitions

# v1.1.5

- fix interaction with show/hide player triggers

# v1.1.4

- fix the wave trail suddenly appearing when ending a level sometimes

# v1.1.3

- fix the trail being invisible for main menu players

# v1.1.2

- fix trail being drawn in non-wave gamemode

# v1.1.1

- fix teleport portal bug

# v1.1.0

- recode everything using a different algorithm, hopefully correct in more cases

# v1.0.3

- fix slant issue

# v1.0.2

- fix interaction with slopes

# v1.0.1

- fix a glitch on the dual wave
- fix the wave trail sometimes connecting to an invalid point from the previous wave

# v1.0.0

- initial release
