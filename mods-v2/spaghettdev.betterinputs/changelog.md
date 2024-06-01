# BetterInputs Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [2.1.0-beta] - 2024-06-01

Robert where update 👀

### Added

- CharNode struct, returned when calling `getCharNodePosInfo` or `getCharNodePosInfoAtLine`

### Fixed

- Text being inserted somewhere completely wrong in TextAreas when highlighting
- Cursor also being positioned somewhere wrong in TextAreas when highlighting

### Changed

- Moved helper types into /src/types folder

## [2.0.0-beta] - 2024-05-31

### Fixed

- Everything (TextArea selection bugs, TextArea highlight sprite going everywhere, and much, much more)

## [1.4.0] - 2024-05-30

### Fixed

- Cursor position funkiness in TextAreas and regular CCTextInputNodes, again
- Cursor position not getting set when using mouse in TextAreas

## [1.3.2] - 2024-05-28

### Fixed

- Cursor position funkiness in TextAreas and regular CCTextInputNodes

## [1.3.1] - 2024-05-27

### Fixed

- More TextArea selection bugs

## [1.3.0] - 2024-05-27

### Fixed

- TextArea selection

## [1.2.0] - 2024-05-26

### Fixed

- Text selection bugs

## [1.1.0] - 2024-05-25

### Fixed

- Text selection and copy/paste shortcuts

## [1.0.1] - 2024-05-26

### Changed

- Logo
- Target geode version (v2.0.0-beta.26 -> v2.0.0-beta.27)

## [1.0.0] - 2024-05-25

### Added

- The project
