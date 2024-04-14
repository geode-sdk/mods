# WholesomeEndTexts Changelog
## v1.1.3
- Finally found a workaround past Cocos2D's tendency to ignore text alignment with multi-line quotes on Android. As such, quotes are no longer forcibly downscaled on Android. If your `bigFont.fnt` is somehow monospaced, that's on you.
## v1.1.2
- Futureproofing the mod against unexpected `m_fields` behavior between Geode versions. Also raised the minimum Geode version requirement.
## v1.1.1
- A single line swap to properly enforce text alignment.
## v1.1.0
- Added compat with GDMO's "Endscreen Info" option.
- Added option to hide QOLMod's "Hide Endscreen" buttons.
- Added "Max Scale" option.
- Note that if you have `relative`'s Custom Endscreen Text mod installed, you *will* need to copy and paste your custom end text messages from the txt file you've set for that mod over to this mod's config, as this mod *will* override those messages.
- *Technically*, this is the initial release for the Geode index, but there have been several notable changes between v1.0.0 and v1.1.0 that it's best to release a new version now to make sure everyone updates to this version.
## v1.0.0
- Initial release (on GitHub).