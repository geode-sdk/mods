# GD-Roulette Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

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
