# v1.0.3
## GDHistory Provider
- Now levels can be copied
## UI
- 'Copy ID' button is renamed to 'Go to Level'
  - This button now goes into Level Info menu, not to the level itself.
- 'Get It' button has been removed
- Level Thumbnails are now removed when they get appeared on the screen
## Error Handlers
- Possible error would be printed after going into the Level Info page instead of immediately returning
### GDHistory Provider
- New descriptive errors:
  - `-7` - GD History's api is down.
  - `-8` - API did not return record data.
  - `-9` - API returned record data with invalid data type.
  - `-10` - API returned record array with zero levels in it.

# v1.0.2
## GDHistory Provider
- Fixed typo
- Feature score is now parsed properly
## UI
- Fixed button placement in the Online layer
- 'Play Level' is now faded if level/record does not have level data
- 'Copy ID' button now is not shown on Android (due to crashes)
- Level thumbnails are now removed automatically
- Level ratings are now removed automatically
## Error Handlers
- '`gmd api error`' now also dumps level string
### GDHistory Provider
- Added error handler for specific private level records

# v1.0.1
### GDHistory
- Fixed HTTP bug
### Base
- Initial release on Android

# v1.0.0
- Initial release for Windows