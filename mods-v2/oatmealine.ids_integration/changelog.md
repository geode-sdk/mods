## v1.4.0-beta.1

Based on `oatmealine.nlw_integration` v1.4.0-beta.2:

> **Experimental release**

- Switches over level name / creator name matching to server-side ID fetching
  - This means all the work is done on the NLW API server rather than the client, but this reverse method of fetching also results in more incorrect guesses
  - However, this should mean levels not on sheets will not be misrecognized as something that is
  - This is experimental, and I can't test every level to make sure the matches are correct, so I'm putting out a beta release. Report any issues you find to me!
- You can now click the tier text to show every level in that tier as a consequence
  - Some tiers don't work, and I'll work on ironing that out soon
- Swap the popout from using `init` to `initAnchored`. Maybe fixes mobile alignment issues?
- Support platformer levels, now that IDS has those

## v1.3.3

Based on `oatmealine.nlw_integration` v1.3.2:

- Send a user agent for requests
  - **In the future, requests before v1.3.2 may become blocked by `nlw-api`.**
- Update icon

## v1.3.2

- The mod works now lmao

## v1.3.1

Based on `oatmealine.nlw_integration` v1.3.1:

- No longer is every unplaced level Fuck tier
  - C++ strings were a mistake
- Non-extreme demons should no longer be given tiers. Hopefully for good this time

## v1.2.1

Based on `oatmealine.nlw_integration` v1.2.1:

- Improve rating string matching algorithm
  - Mystic will no longer be mismatched to Mystic Bounds

## v1.2.0

Initial release, based on `oatmealine.nlw_integration` v1.2.0