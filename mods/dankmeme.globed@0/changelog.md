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