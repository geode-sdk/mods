# GD-Roulette Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [2.0.4] - 2024-03-13

### Added

- `RLLoadingCircle`, a better LoadingCircle lol

### Changed

- Cleaned up `#include`s in header files

### Fixed

- 5 Character limit in `RLIntegerInputLayer`
- `LoadingCircle` in wrong position on Android

## [2.0.3] - 2024-03-09

### Changed

- No longer use `geode::Notification`, now use `rl::utils::createNotificationToast`
- How levelIDs are stored when in LevelInfoLayer (they no longer are)

### Fixed

- Weird 5th arg in `TextAlertPopup::create`

## [2.0.2] - 2024-03-06

### Added

- `#include` directives to the `/custom_layers`
- Platform name to `RLRouletteInfoLayer`
- `RLDifficultyNode` supports epic, legendary and mythic now
- `rl::utils::getFeatureStateFromResponse`

### Changed

- Renamed RLDemonSelectLayer to RLDifficultySelectLayer
- Made RLDifficultySelectLayer dynamically made (RLDifficultySelectInfo)
- How touch prio is handled in RLRouletteLayer
- Made the difficulty buttons in RLDifficultySelectLayer in another menu
- Refactored RLDifficultySelectLayer.cpp
- Use structured bindings (i forgor they existed)
- `RLDifficultyNode` now inherits from CCNodeRGBA (rookie mistake)

### Fixed

- Empty list id crash on Android (probably)
- Show options sprite being set even if the info icon was never clicked
- `RLDifficultyNode::setColor` being weird
- Difficulty not being highlighted when changing the list multiple times

## [2.0.1] - 2024-03-03

### Fixed

- `RouletteManager` not getting new keys because it just assumed they existed prior

## [2.0.0] - 2024-03-01

GD-Roulette commit everything at once challenge (mildly possible)

Notable changes:

- MacOS support
- GD Lists option
- Ability to pause when in a round of roulette
- Bugs & crashes

### Added

- rtrp library, that parses Geometry Dash's server responses, made by yours truly
- MacOS support
- `RLDemonSelectLayer`, a layer that lets you select a demon difficulty (appears when clicking the demon plus button)
- `IntegerInputInfo::show_arrows` bool
- `RLDifficultyNode`, a custom node that's basically `GJDifficultySprite` but better IMO
- `ListFetcher::level_pair_t`, an `std::pair` of a LevelObject and a CreatorObject
- `ListFetcher::getRandomGDListLevel`
- `ListFetcher::GJ_SECRET`, `ListFetcher::GJ_LEVELS_URL`, `ListFetcher::GJ_LISTS_URL`, `ListFetcher::GJ_LEN_QUERY`, `ListFetcher::DEMONLIST_URL`, `ListFetcher::CHALLENGELIST_URL`, `ListFetcher::m_cDemonDiffToFilter`, `ListFetcher::m_cachedGDListID`, `ListFetcher::m_cachedGDListLevelIDs`, `ListFetcher::getDifficultyQuery(GJDifficulty)`
- `RWDI_MODE` macro when compiling in RelWithDebInfo
- GD Lists as a list option
- Info icons to list checkboxes in `RLRouletteInfoLayer`
- Visual indicator of selected list (except GD List)
- Node IDs to RLRouletteInfoLayer
- Node IDs to RLRouletteLayer
- Ability to Pause or Quit when closing RLRouletteLayer
- `RLRouletteLayer::getDifficultyButton`, `RLRouletteLayer::setDifficultyButtonColor`
- JSON arrays are checked on launch in `RouletteManager`'s ctor
- `RouletteManager::isPaused`, `RouletteManager::gdListID`, `RouletteManager::previousDifficulty`, `RouletteManager::previousDemonDifficulty`, `RouletteManager::getDifficultyFromSaveContainer()`
- `rl::constants` namespace
- `rl::utils::createLevelFromResponse()`, `rl::utils::getCreatorFromLevelResponse()`, `rl::utils::getDifficultyFromResponse()`
- Geode 2.0.0-beta.21 support
- Some missing node IDs to `RLRouletteLayer`
- Some colors to some layers

### Changed

- Rely on Geometry Dash's servers instead of GDBrowser's API (this was long overdue)
- Renamed `BaseCustomLayer` to `BaseCustomAlertLayer`
- Prefixed all custom layers/nodes with `RL`
- Renamed `ConfirmationAlertInfo::onYes` to `RLConfirmationAlertInfo::onBtn1`
- Renamed `ConfirmationAlertInfo::onNo` to `RLConfirmationAlertInfo::onBtn2`
- Renamed `RLRouletteLayer::onDifficultyChosen` to `RLRouletteLayer::onDifficultyButton`
- Renamed `roulette` namespace to `rl`
- Pass `ConfirmationAlertInfo` into the `create` method instead of `setup`
- `IntegerInputInfo::starting_value` is now an `std::optional<int>`
- rouletteButton `CreatorLayer`'s CCMenu is now positioned based on the window's size
- All `as` back to `static_cast`s because yes
- Renamed `ListFetcher::normalListMaxPage` to `ListFetcher::m_cNormalListMaxPage`
- Updated `ListFetcher::m_cNormalListMaxPage`
- All `ListFetcher`'s methods take a `ListFetcher::level_pair_t` instead of a `matjson::Value`
- `ListFetcher::getRandomNormalListLevel` is passed a GJDifficulty instead of an int
- How `RLRouletteLayer::onDifficultyButton` handles stuff
- `RLRouletteLayer::getRandomListLevel` is passed a GJDifficulty instead of an int
- How coins are positioned in `RLRouletteLayer` (they're now based on the difficulty node's position)
- Some info about the info icons in ABOUT.md
- How touch priority is handled in BaseCustomAlertLayer
- No longer use `geode::cocos::handleTouchPriority`

### Fixed

- Made the rouletteButton a bit better code-wise (still sucks)
- Potential crash when modifying `LevelInfoLayer` of a platformer level
- Potential crash when modifying `PauseLayer` of a platformer level
- Invalid page when searching for a level in `ListFetcher::getRandomNormalListLevel`
- Dev macro (RWDI_MODE)
- Demon plus button visible in Demon List and Challenge List modes
- Weird static variable swap stuff in `RLConfirmationAlertLayer` and `RLIntegerInputLayer`
- Odd way of resetting all `CCMenuItemToggler`s after being toggled
- Clicking the level's name/creator/id not copying it to the clipboard
- Potential crash if `RLRouletteLayer::m_level` is empty (highly situational)
- Geode invalid tags
- Touch Prio on android :heart:

## [1.6.2] - 2024-02-09

### Fixed

- Crash when leaving LevelInfoLayer

## [1.6.1-beta.3] - 2024-02-07

### Changed

- No longer target any Node-IDs version because that's broken. Instead, target v1.3.0

## [1.6.1-beta.2] - 2024-02-07

### Changed

- Actually target any Node-IDs version that matches or is greater than 1.3.0, previous version targeted v1.1.4

## [1.6.1-beta.1] - 2024-02-07

### Added

- Auto pause option
- Some IDs to layers that are modified

### Changed

- Target Geode 2.0.0-beta.16
- Some `static_cast`s to `as`
- CHANGELOG.md layout to "Added", "Changed" then "Fixed"
- Target any Node-IDs version that matches or is greater than 1.3.0
- Changed some for loops to getChildByID
- Renamed RouletteManager::lastLevelID to currentLevelID
- Renamed RouletteManager::lastLevelPercentage to currentLevelPercentage
- Removed Node-IDs dependency in CMakeLists.txt
- Removed RouletteManager::levelCreatorName
- Renamed about.md to ABOUT.md

### Fixed

- Goal percentage appearing in a level that isn't the current roulette level

## [1.6.0-beta.4] - 2024-02-06

### Fixed

- Platformer levels appearing in the roulette

## [1.6.0-beta.3] - 2024-02-04

### Changed

- Geode 2.0.0-beta.15 support

## [1.6.0-beta.2] - 2024-02-04

### Changed

- assets/GD-Roulette.png
- Removed 1 unnecessary objectAtIndex

### Fixed

- Crash when on a fresh install of GD-Roulette

## [1.6.0-beta.1] - 2024-02-04

### Added

- Android support (?)
- Error text when ListFetcher fails to fetch a link
- RouletteLayer pointer member to RouletteManager
- Array verifier to assure selected difficulty/list is correct (cant select multiple at once, maybe for a future update?)
- Choosing a list highlights a difficulty that matches said list

### Changed

- about.md
- Logo
- RouletteManager to be an inline global variable instead of that broken define system
- Removed CustomDirector
- Made selecting a list change the selected difficulty (only visual)
- Renamed RouletteManagerStruct to RouletteManager
- Renamed RouletteManager's variable name to g_rouletteManager
- Cleaned up include directives

### Fixed

- Crash when clicking Reset after ListFetcher fails
- Bugs

## [1.5.0-beta] - 2024-02-03

### Changed

- CURL for Geode's web::AsyncWebRequest
- nlohmann::json for matjson
- Move from CCString::createWithFormat to fmt::format
- Move from JsonManager to Geode settings/save data

### Fixed

- Crashes

## [1.4.0-alpha] - 2024-01-31

This release is very unstable and doesn't get past the "Start" button.

### Added

- 2.2 support
- Geode support

## [1.3.0] - 2023-12-17

Last update before 2.2. I might update this to 2.2 if I have enough free time.

### Added

- Added a confirmation dialogue layer that is used when closing the RouletteLayer while playing
- Added a reset method to the RouletteManager struct
- Added an OK button to the IntegerInputLayer

### Changed

- Moved CustomLayer and its inheriting classes to /src/custom_layers
- Separated each bunch of nodes to unique CCMenus
- Changed RouletteInfoLayer's text nodes from CCLabelBMFont to TextArea
- Repositioned the RouletteInfoLayer's toggles
- Renamed RouletteInfoLayer::onSkipsButton to onNumSkipsButton
- Renamed RouletteManager::skipsCount to skipsUsed
- RouletteLayer.difficultyToTag is now const
- Phased out use of std::to_string in favor of CCString::createWithFormat (with the exception of ListFetcher)
- Removed unused parameters' names in onXButton functions
- IntegerInputLayer's information is dynamic instead of hard coded
- Renamed CreatorLayer's ButtonsClass to RouletteButton
- Refactored CreatorLayer.cpp

### Fixed

- Fixed ConfirmationAlertLayer result getting ignored
- Fixed touch events not getting dispatched from the nested RouletteLayer CCMenus
- Fixed RouletteButton's CCSprite being too big on resolutions other than High
- Fixed the roulette level's author name being removed

## [1.2.1] - 2023-12-10

### Added

- Added a 1s pause after player death while playing a level

### Changed

- RouletteInfoLayer::createToggler's definition from RouletteLayer.cpp to RouletteInfoLayer.cpp
- Removed duplicate code ln. 402-403 -- ln. 409-410 in RouletteLayer.cpp
- Removed duplicate code ln. 436-437 -- ln. 447-448 in RouletteLayer.cpp

### Fixed

- Fixed JsonManager overriding saved values

## [1.2.0] - 2023-12-06

### Added

- Added a json manager (to save options)
- Added a percentage goal besides the LevelInfoLayer percentage text
- Added a percentage goal in the PauseLayer

### Changed

- Separated the layers contained in the RouletteLayer.cpp file into sub-files

### Fixed

- Fixed RouletteManager not managing data correctly after JSON saving was added
- Fixed demonDiffArr resetting everything to false when RouletteLayer::onClose is called

## [1.1.7] - 2023-10-29

### Added

- Added a DEV_CONSOLE macro enabled only when compiling RelWithDebInfo
- Added a check for MegaHack v7 to change the roulette button's position
