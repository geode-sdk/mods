# Changelog

## v1.5.2
 - Fix unpausing with space also causing the player to jump
 - Add missing "Pan editor while swiping" editor keybind
 - Add missing "Transform" editor keybind

## v1.5.1
 - Fix not being able to hold from respawn in PlayLayer

## v1.5.0

 - Add editor save & load position keybinds
 - Fix a lot of the internal implementations of keybinds to just use GD's implementations, potentially fixing a bunch of inconsistencies in the editor

## v1.4.0
 
 - Fix being able to reset levels during level end animation
 - Remove editor half-move and big-move keybinds, since those are not in the vanilla game and as such should be implemented through mods instead

## v1.3.3

- Fix editor keybinds
- Add F-Keys to editor keybinds
- Add half moves and big moves to editor keybinds

## v1.3.2

- Add DPad Up as default for P1 Jump
- Make keybind info popup wider

## v1.3.1

- Changed the name of the default platformer binds (move left right)
- Made platformer move binds unrepeatable
- Added "W" for Jump P1 as a default
- Fixed non-repeatable binds repeating (a lot)
- Fixed default platformer move binds for P2

## v1.3.0

- Fix controller support
- Add sprites for missing controller buttons (RB, RT, LB, LT)
- Improve controller sprite display in the keybind picker
- Add platformer keybinds
- Add reset, full reset, and toggle hitboxes (this one is experimental)

## v1.2.4

- Add 2.204 support

## v1.2.3

- Fix issues caused by the impostor PlayLayer bug

## v1.2.2

- Fix jump key not working after a level restart

## v1.2.1

- Fix issues with MegaHack
- Add EditorUI controller keybinds
- Improve controller compatibility in UILayer

## v1.1.2

- Fix crashes on exit for Windows

## v1.1.1

- Fix issues on MacOS
- Make repeatable binds false by default