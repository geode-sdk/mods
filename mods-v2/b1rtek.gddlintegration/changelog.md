# v1.1.2
- Going back from search results goes back to the right place (finally!)
- Added a missing alert saying that the rating is still loading (while it's actually loading)
- Updated the search menu to be compatible with the new GDDL API version

# v1.1.1
- The old search menu can be opened with a click on a green arrow on the bottom right of the search popup
- Android users can finally input the correct amount of characters into text fields
- Old tier label displays on top of the epic/legendary/mythic fire
- The tier button/label is given a texture/color and content that matches the tier in the local cache, making it feel like the rating is instantly loaded

# v1.1.0
- The search menu has been replaced by a much better one that allows the user to take full advantage of the GDDL API
- Results in the GDDL Demon Split displayed in the level list after clicking a tier are now accurate according to the data in the GDDL API (that's why the numbers might not match, as the counts are generated using local cache)
- The GDDL Search button can be now moved down (look in settings)
- The GDDL Tier button on the level info page can be replaced again with a label, and it can be moved down (although it might overlap with the diamonds label in gauntlets and weeklies)

# v1.0.5
- Added an option to search for levels by tier
- You can find that in the search menu, there's a GDDL button located on the right side

# v1.0.4
- Added an option to move the tier rating button next to the level name (either on the right or the left side), the placement can be controlled with dedicated settings
  - [feature suggestion by thesuperjepphykiller](https://github.com/B1rtek/Geode-GDDLIntegration/issues/6)
- GDDL Demon Split info popup has more information now
- Info showed after clicking the tier button on the level page has <cp>c</c><cr>o</c><co>l</c><cy>o</c><cg>r</c><cj>s</c> now
- The game shouldn't crash anymore after opening the profile page now (added `geode.node-ids` as a dependency)
  - [bug report from Lexicon](https://github.com/B1rtek/Geode-GDDLIntegration/issues/7)

# v1.0.3
Added the *GDDL Demon Split* screen, which shows how many demons of each tier you've beaten (according to a list that gets cached every 7 days)

![And it looks like this](b1rtek.gddlintegration/split.png)