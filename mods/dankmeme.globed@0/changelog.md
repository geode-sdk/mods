# v0.4.2

* Potentially fixed some bugs specific to Mac
* Auto music sync when spectating now works on Android

# v0.4.1

* Fixed the random safe mode bug when completing a level (oops)
* Spectate button now unpauses the game automatically
* Fix music-related spectating bugs
* Fix spectating being buggy in practice mode or with start pos
* Fix death effects not properly rendering
* Add death sound effect when spectating
* Spectating is now functional on Android

Other (mostly minor) fixes:

* Balls are now appropriately sized
* Added an icon for indicating that a player is paused
* Changed the way icons are shown above player heads
* Server levels button is hidden if not connected to a server
* Position of the refresh button is now consistent between servers menu & server levels menu
* No longer playing death effects on the dual icon
* Practice and restart buttons no longer do anything when spectating
* added even more bugs!

# v0.4.0

* Added <cg>spectating</c>!!!! (it actually works!!!!) (experimental!!!!)
* Added <cy>death effects</c>, and two new settings for controlling them
* Added <cj>level ending animation</c>
* Added a setting to disable the overlay text when in a custom level or disconnected
* Ported the mod to <cg>Android</c> for the upcoming Geode 1.4.0 release
* Fixed major bugs on Mac
* Added glow to the cube passenger inside ship & ufo
* Added glow to the icons in the spectate list
* Fixed dash rotations being buggy
* Removed the default mini icons setting because it didn't work properly

Due to protocol changes, this is a required update. Without it you won't be able to connect to official servers.

# v0.3.2

* Improve the progress indicator
* Progress line uses player's secondary color by default now, can be changed in settings
* Player list now shows yourself
* Player list hidden on custom levels or when disconnected
* The server levels button position can now be customized
* Fixed a crash when leaving the server levels menu too quick

# v0.3.1

* Hide progress indicators of other players when the progress bar is hidden
* Add an option to change the size of the progress indicator
* Add an option to show your own icon below the progress bar too
* Add lines to the progress indicators
* Add a button on the level page to open the server levels list
* Fixed a very obscure crash
* Fixed a small Mac issue

# v0.3.0

* Made it so that you can see other players move while paused (thanks mat for helping to figure it out)
* Changed the player progress indicator to a much prettier one
* Mac support (largely untested, thanks a lot to Firee for helping with it)
* Added glow for player icons
* Changed interpolation (again?) to make other players move smoother (maybe?)
* Fixed some other bugs

Due to protocol changes, this is a required update. Without it you won't be able to connect to official servers.

# v0.2.1

* Made the server levels list much faster and more efficient (thanks to Cvolton and Alphalaneous)
* Fixed a typo in mod's description (thanks Aktimoose)
* Made it impossible to get a million error popups get thrown at you
* (hopefully) controller back button works now to exit menus (made exclusively for Cvolton)
* Added better validation on the server for invalid names and icons
* Tweaked mod logo & menu icon again (thanks to Alphalaneous and ca7x3)

# v0.2.0

## Lag is no more (sort of)

This update brings an overhaul to interpolation, and your game should be much smoother provided a stable ping, even if it's a high one.

There have been a lot of changes, so if you find any issues, feel free to contact me. You can do it on discord @dank_meme01, or in github issues if you feel like it, for some reason.

Detailed list of changes:

Interpolation related:

* Completely overhauled interpolation, rewritten with the mathematical formula `lerp` instead of own formulas
* Added timestamps to `PlayerData` packets to try and make other players' movement more accurate
* Removed the PPA engines setting
* Tried to counteract packet loss by applying extrapolation if needed
* Made packet receiving more efficient (1 packet = 1 datagram instead of 2)
* Remove Y rotation since X and Y rotations are generally always equal to each other

Other changes:

* Added colorful names for people who helped me or supported me, can be disabled in settings
* Changed the mod logo (and menu icon) (thanks [@ca7x3](https://twitter.com/ca7x3) :D)
* Made the menu icon change color depending on whether you are connected to a server or not
* Made some error messages a bit nicer
* Introduced more bugs
* Bump the protocol version to 5

The last change means you have to update the mod in order to use any of the official servers.

# v0.1.3

* Improved interpolation for greater smoothness
* Blocked connecting to the server with no account
* Made it harder for data corruption to cause a crash
* Fixed some grammatical errors
* Other minor fixes

# v0.1.2

Initial release.