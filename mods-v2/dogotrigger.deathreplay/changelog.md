# v1.2.0 Beta 5
### Gameplay Changes
 * New setting: `Record Players in Globed`
   - This setting allows Death Replay to record online players if enabled.
   - **Disabled by default**.
   - Fixes `#6`.
### Technical Changes
#### Since v1.2.0 Beta 1
 * `playTime` parameter is fully ignored if level was not released and updated since 2.2+ release
### Mod Description Changes
 * Changelog in `README.md` has been updated

# v1.2.0 Beta 4
### Gameplay Changes
 * 'X' sprite is now half visible
### Techinical Changes
 * Code is cleaned up a bit
### Mod Description Changes
 * Repository link is updated to use proper repo name

# v1.2.0 Beta 3
### Gameplay Changes
 * Pressing ESC on removing Death Replay file popup now doesn't do anything (#2)
### Techinical Changes
 * Death particles are now spawned properly
 * SDK has been updated to `v2.0.0-beta.12`
 * Ghost's recording now includes Player scaling

# v1.2.0 Beta 2
### Gameplay Changes
 * Now you can remove Death Replay file for any level by clicking to red back arrow button
### Technical Changes
 * SDK has been updated to `v2.0.0-beta.11`
 * Bugfixes
 * playTime parameter is now fully ignored if played level has been created/updated last time before 2.2
 * Debug output has been removed
### Mod Description Changes
 * `changelog.md` formatting has been changed a little bit

# v1.2.0 Beta 1
### Gameplay Changes
 * Ghost has been temporarily disabled; it's very broken in 2.2
### Technical Changes
 * SDK has been updated to `v2.0.0-beta.9`
 * Ghost now waste less CPU time when its hidden than in DR v1.1.0
 * Death Replay level file now has new parameter - playTime
   - `playTime` parameter is fully ignored while being in Platformer mode.
   - Normal Mode can use playTime parameter if it possible.

# v1.1.1
### Gameplay Changes
 * Fixed bug where Ghost didn't get hidden when he was said to
 * Ghost now can be attached to any number of players so the Dual Mode is now working properly
### Technical Changes
 * SDK has been updated to `v1.3.5`
 * Ghost now doesn't waste CPU time and RAM when its hidden
### Mod Description Changes
 * `README.md` now has mod information and changelog

# v1.1.0
### Gameplay Changes
 * Added the Ghost player
   - This Ghost shows after your death or level completion and replays previous inputs.
   - Ghost is hidden by default. You can make it visible in the mod settings.
### Techincal Changes
 * SDK has been updated to `v1.3.3`
 * Source code now has Logo's GIMP project file
 * Mod now doesn't use child indexer
### Mod Description Changes
 * Changelog now looks better

# v1.0.2
### Mod Description Changes
 * Added changelog

# v1.0.1
### Techincal Changes
 * Removed debug printf
 * Changed save path to geode's

# v1.0.0
 * Initial release