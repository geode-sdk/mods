## Death Sound Randomizer Changelog
# v1.1.0
- Android support!
- Moved sounds folder to config dir (pencil icon thing) (your folder will be automatically moved!)
- Death sounds are cached and preloaded when loading a level (no more lagspikes when playing a long sound for the first time!)
- Now using std::mt19937 rng instead of rand() (aka less repeated sounds)
- Killing icons in the menu now plays random death sounds!
- Added "Force Death SFX" option
- Added "Stop Death SFX on Respawn" option (enabled = default gd behaviour)

# v1.0.0
- Initial release