# ErysEdits Changelog
## v1.1.2
- (Hopefully) fix a rare crash with LoadingLayer.
- Added mods list copying functionality to the `Level End Screen: Show Mods List` setting.
- Bump Geode minimum version to 2.0.0-beta.26.
- Bump Custom Keybinds minimum version to v1.5.7. *[Windows only.]*
## v1.1.1
- Fix a silly bug with the debug text's `Compact "Gameplay" Section` setting. Oops!
## v1.1.0
- New slider settings: `Always Active LDM` and `Level End Screen: Show Mods List`. Make sure to read their config descriptions!
- A few miscellaneous settings for tidying up the icon kit. 
- Removed the setting that forces the player death SFX to play. Please use similar settings in v1.1.0 of Adam729's Random Death Sounds mod instead.
- Remove disabling the platformer cube jump squishing animation. Please use similar settings in v1.2.0 of RayDeeUx's BreakingPlatforming mod instead.
- Clarify descriptions when levels appear to have an empty description despite proven otherwise, especially when browsing level lists.
- Fix an issue where SFX in some levels would infinitely loop. Thank you, Aktimoose, for bringing this to my attention, and deepest apologies for rejecting your original claims. I hope this apology and this update is compensation enough for my harsh behavior at the time.
- Unfortunately, there's still incredibly specific edge cases where SFX *can* loop infinitely while using this mod, so a config description has been added to the relevant spot.
- Recategorized a few settings.
- Added punctuation to changelogs.
- Bump Geode minimum version to 2.0.0-beta.25.
- Bump Node IDs minimum requirement to v1.9.1.
- Add keybinds for the level search menu, gauntlets menu, and icon kit. *[Windows only.]*
- Add keybinds when viewing comments in a level/viewing comments by a specific user. *[Windows only.]*
- Add keybinds to open the settings menus for both Geometry Dash and this mod. *[Windows only.]*
- Add a keybind to open your Geode custom keybinds. *[Windows only.]*
- Add an additional keybind to save and exit an editor level. *[Windows only.]*
- Add a keybind to open the Geode mods list. *[Windows only.]*
- Add keybinds to (toggle between viewing, creating new, or viewing uploaded) custom levels and level lists. *[Windows only.]*
- Add a keybind to close the level editor's pause menu. *[Windows only.]*
- Categorized keybinds properly. *[Windows only.]*
- Bump Custom Keybinds minimum requirement to v1.5.6. *[Windows only.]*
## v1.0.2
- Rebuild the mod due to *someone* mangling up `FLAlertLayer` codegen for Android.
- Fix funky text scaling behavior in `FLAlertLayer`s with scrolling enabled by default.
## v1.0.1
- Less restrictive width caps on `FLAlertLayer` (anything wider than 420 units before being modified by ErysEdits is unaffected).
- "Brought back" Soggy Mod re-compatibility.
## v1.0.0
- Initial release (on GitHub).