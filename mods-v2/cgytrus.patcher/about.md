# Simple Patch Loader
A simple patch loader for Geode.
Supports MHv5, MHv6, GDHM and its own format.
Integrates with MHv7 if installed.

## Usage
Press **[Caps Lock]** to open the menu.

Click "Open Patches Folder" and put your patch files in there:
- root folder contains patches designed specifically for Simple Patch Loader
- `mhv5` sub-folder contains patches designed for Mega Hack v5
- `mhv6` sub-folder contains patches designed for Mega Hack v6
- `gdhm` sub-folder contains patches designed for GD HackerMode
- `old-gdhm` sub-folder contains patches designed for old versions of GDHM

### For Windows users
You can download MHv5's hacks directly from SPL using the "Download MHv5 hacks" button.

You can also download [GDHM](https://youtu.be/x0KJ9Rq5Xw0) (see video description)
and copy the .json files from `.GDHM/mod` into `gdhm` in SPL's patches folder.

### Patch Format
- The file name is the **category ID**
- The file in **JSON format**
- Root object contains `name` and `patches`
  - `name` is a string which is the **category name**
  - `patches` is an object containing the **patches**
    - The keys are **patch IDs**
    - The values are objects, containing `name`, `description` and `address`
      - `name` is the **patch name**
      - `description` is the **patch description** shown when *hovering* in the menu (doesn't work when SPL is used with MHv7)
      - `address` is an object, containing the **actual patches**
        - The keys have the following syntax: `module signature offsets`
          - (optional) `module` - base module name (such as `libcocos2d.dll`), defaults to the base module (GD itself)
          - (optional) `signature` - signature to use to scan for an address in the selected module, sets current address to the found address
          - `offsets` - offsets from the current address
            - uses [Reverse Polish Notation](https://en.wikipedia.org/wiki/Reverse_Polish_notation), so `0x3 0x1 -` results in `0x2`

```json
{
    "name": "Test",
    "patches": {
        "test-patch": {
            "name": "Test Patch",
            "description": "old accurate percentage",
            "address": {
                "0x208114": "C7 02 25 66 25 25 8B 87 C0 03 00 00 8B B0 04 01 00 00 F3 0F 5A C0 83 EC 08 F2 0F 11 04 24 83 EC 04 89 14 24 90",
                "0x20813F": "83 C4 0C"
            }
        },
        "test-2": {
            "name": "Test 2",
            "description": "new accurate percentage",
            "address": {
                "[33 C9 F3 0F 10 00 F3 0F 5E 87 B4 03 00 ?? ?? ?? ?? 05]": "F3 0F 10 00 F3 0F 5E 87 B4 03 00 00 BA ref:0x2E65C0 F3 0F 59 02 0F 2F 02 76 04 F3 0F 10 02 8B 87 C0 03 00 00 8B B0 04 01 00 00 F3 0F 5A C0 83 EC 08 F2 0F 11 04 24 68 ref:0x2881B0",
                "0x20813F": "83 C4 0C",
                "0x2881B0": "25 2E 32 66 25 25 00"
            }
        },
        "test-3": {
            "name": "Test 3",
            "description": "new accurate percentage but with offsets",
            "address": {
                "[C9 F3 0F 10 00 F3 0F 5E 87 B4 03 00 ?? ?? ?? ?? 05] 0x1 -": "F3 0F 10 00 F3 0F 5E 87 B4 03 00 00 BA ref:0x2E65C0 F3 0F 59 02 0F 2F 02 76 04 F3 0F 10 02 8B 87 C0 03 00 00 8B B0 04 01 00 00 F3 0F 5A C0 83 EC 08 F2 0F 11 04 24 68 ref:0x2881B0",
                "0x20813F": "83 C4 0C",
                "0x2881B0": "25 2E 32 66 25 25 00"
            }
        },
        "test-4": {
            "name": "uwu :3",
            "description": "no paritcles",
            "address": {
                "libcocos2d.dll 0xB76C5": "31 F6",
                "libcocos2d.dll 0xB8ED6": "00"
            }
        }
    }
}
```
