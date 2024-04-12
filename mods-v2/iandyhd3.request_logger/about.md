# Request Logger

Logs every request made through cocos2dx to the console (default) or to a file (enable in options)

Make sure to have geode console enabled, otherwise you won't see anything!

## Settings

Several things are customizable:
- log to console
- log to file
- key/param console color
- post body key color
- post body value color
- hide password (gjp2)

Example:
```
Url: https://www.boomlings.com/database/getGJDailyLevel.php
Status: 200
Request Body: gameVersion=22 binaryVersion=40 udid=ffffffff-88c5-aa6d-ffff-ffffcd72151b uuid=4460760 accountID=1688850 gjp2={hidden} secret=Wmfd2893gb7 type=0
Response: 2693|13437
```