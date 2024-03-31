# ErysEdits
Several mods I would've made into smaller standalone mods when I was an ignorant Geode developer. (And I still probably am by several accounts, but who's keeping track? `/j`)

Not all features of ErysEdits are available across all platforms; check your settings for this mod after installing to verify.

## Features
- Various Info Label tweaks, including improved readibility, conditional displays, and debug text logging

![demoOne](raydeeux.erysedits/demoOne.png&scale:0.75) ![demoOnePointFive](raydeeux.erysedits/demoOnePointFive.png&scale:0.75)
![demoOnePointSeventyFive](raydeeux.erysedits/demoOnePointSeventyFive.png&scale:0.75)
![demoOnePointEightHundredSeventyFive](raydeeux.erysedits/demoOnePointEightHundredSeventyFive.png&scale:0.75)

- Viewing level descriptions from level lists and daily/weekly levels (compatible with nearly every possible mod that edits the LevelCell, including Cvolton's BetterInfo + Compact Level Lists, cdc's Level Thumbnails, n's Level Pronouns, and dankmeme's Globed)

![demoTwo](raydeeux.erysedits/demoTwo.png&scale:0.75)
![demoTwoPointFive](raydeeux.erysedits/demoTwoPointFive.png&scale:0.75)
![demoTwoPointSeventyFive](raydeeux.erysedits/demoTwoPointSeventyFive.png&scale:0.75)

- Compact local levels list (with some code borrowed from Cvolton, compatible with LevelSize by hiimjustin000)

![demoThree](raydeeux.erysedits/demoThree.png&scale:0.75)

- Hide "Level Complete" visuals (except particles, use your local mod menu to hide those)

![demoFour](raydeeux.erysedits/demoFour.png&scale:0.75)

- Disabling the cube jump animation in platformer levels (hitbox trail for reference)

![demoFive](raydeeux.erysedits/demoFive.png&scale:0.75)

- Compact view of user profile comments/posts

![demoSix](raydeeux.erysedits/demoSix.png&scale:0.75)

- Various FLAlertLayers tweaks (including wider alerts, smaller, text, and scrollable text)

![demoSeven](raydeeux.erysedits/demoSeven.png&scale:0.75)

- Hidden progress bar and percentage on unverified local levels
- Force levels to stop music on death
- Force levels to play your death SFX on death (compatible with Adam_729's Random Death Sounds and ControlVanillaSFX, see mod settings for more details)
- Various keybinds to make navigating Geometry Dash feel a lot less repetive (Ctrl + S to save, Ctrl + R to refresh, Alt + Left/Right to navigate between layers with pages, Shift + Left/Right to go to the first or last page, etc)
- Requiring Shift key to enter shops and vaults (to avoid changing menu loop music)
- Disable Shake, Pulse, Area Tint, SFX, and Edit SFX triggers

## Special Thanks
- [acaruso](user:25012294), for moral support + massive optimizations in codebase during development
- [Cvolton](user:761691), for lending their C++ knowledge and allowing me to reuse/adapt some of their code from BetterEdit, Misc Bugfixes, and Compact Lists
- [Alphalaneous](user:1139015) and [dankmeme](user:9735891), for supplemental CMake/C++ expertise
- [SpaghettDev](user:7670168) and [Prevter](user:7696536), for finding memory address bindings that fully fleshed out some features (`0x305630` for `SecretLayer2::create()`;  `0x276180` and `0x276170`, for `LikeItemLayer::onDislike()` and `LikeItemLayer::onLike()` respectively)
- [Cooper](user:21207551), for allowing me to reuse code for custom setting headers
- [CatXus](user:14467409), for extensively testing this mod on Android, and for helping me sing "You Are a Pirate" from LazyTown ;)
- [sofabeddd](user:7976112), for the occasional reality check

This [Geode mod](https://geode-sdk.org) is licensed under LGPLv2.