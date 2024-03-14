# Version 1.3.1
- Code optimization
- Added a string ID to the label
- Improved the mod's description in the README.md, the about.md and the mod.json files

# Version 1.3.0
- Added the editor time setting
- Added the editor time (+copies) setting
- Added the total attempt setting
- Added the total jumps setting
- Added the clicks setting
- Added the best time setting
- Fixed the object count setting being locked at 65535 objects (might need to refresh the level if it was not already in the local cache)
- Removed try/catch blocks to avoid crashes on Android
- Changed logs debug to info
- Made logs show the level and its author
- Removed a duplicate main.cpp (which fixed macOS build failing, which means macOS support is back!)
- Fixed the mod getting informations about the level and displaying them even if every settings were disabled

# Version 1.2.1
- Optimized the code for many things: Feature state, Object count and Game version (Thanks VolcaroCham!)
- Levels before 1.7 will be labeled "Pre-1.7"

# Version 1.2.0
- Added the game version settings/stats
- Added GitHub issues
- Optimized the code
- Added logs
- Added error handling
- Added more notes to make the code more understandable
- Made object count display “Unknown” if for some reason the object count was at 0
- Added changelog.md
- New logo by freadfries!

# Version 1.0.1
- Added the utility and interface tags
- Added an option to change the text color