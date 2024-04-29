# Pickups Across Sessions 

This mod allows you to save item ids across sessions, so you can save your pickups ids and use them in any levels you publish from your account. Item IDs are saved with a string ids system and they are saved by account ID, this poweful system allows you to save and read item ids from any level publisehd from your account.

## How does it work?

When you exit a level, the mod will save the specified persistent item ids to a file. When you enter a level or respawn, the mod will read the file and restore the item ids.

## Usage

It is important to understand that the string ids system is account based, this means that you can save different item ids in level A, and you can read/modify them in level B. This works across all levels you publish from your account. 

All the configuration of the mod is done via text objects. In order to enable the mod in your level add a text object with this exact string in lowercase: `@perspickup`. Use the command `@{itemid} {name}` to map an item id to a variable. For example `@10 counter` maps the item id `10` to the id `counter`. As the string ids are account based, we can use the same id in a different level and load it in any other item id we want. `@5 counter` would restore the previously stored `counter` value in the item id `5`. 

## Limitations

At the moment, item ids are not restored before the first frame triggers are executed, which means you need a small delay to read restored item ids

## Why is all done with text objects?

In summary, a key design goal of this mod is to remain easily adaptable to future versions of Geometry Dash. While not ideal, the current text object system provides a straightforward and easily updatable approach.


## Test levels
`104430770`, `104430764`

## Bugs/Suggestions

Open an issue or let me know on discord