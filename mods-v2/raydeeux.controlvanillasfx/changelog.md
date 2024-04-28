# ControlVanillaSFX Changelog
## v1.3.2
- Fix an issue where SFX in some levels would infinitely loop. Thank you, Aktimoose, for bringing this to my attention, and deepest apologies for rejecting your original claims. I hope this apology and this update is compensation enough for my harsh behavior at the time.
- Bring back the rare edge case where `reward01.ogg` would play in the basement. RobTop's infinite wisdom overflowed into the negatives when writing 2.2, allowing him to call the most dangerous FMODAudioEngine function when playing that SFX. Hooking that particular FMODAudioEngine function ends up causing some SFX to loop forever in levels. At this point, I'd suggest grabbing a texture pack to mute that sound effect.
- Increase minimum Geode requirement to `beta 25`.
## v1.3.1
- Fix an issue with SFX not playing at all on Android. ***THANK YOU WEEBIFY!***
## v1.3.0
- Android support.
- Bump minimum Geode version requirement.
- Fix a rare edge case where something similar to `reward01.ogg` would play despite volume controls.
## v1.2.0
- Move vanilla SFX to a different FMOD audio channel (with help from Weebify).
- Remove the "speed" config option as a result.
## v1.1.0
- Remove unintended side effects with Beat & Co.'s Click Sounds mod.
## v1.0.0
- Initial release.