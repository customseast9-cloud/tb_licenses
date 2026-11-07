# tb_licenses - QBCore License System

## Overview

tb_licenses is a QBCore-based FiveM resource that allows players to purchase, manage, and renew various licenses (e.g., driver's license, CDL, hunting, fishing, pilot, etc.) at a designated PED location. The system enforces that a player must have a driver's license item before purchasing any other license.

## Features
- Buy and renew multiple license types (driving, commercial, recreational, etc.)
- License info stored as items with personal data (name, birthdate)
- Requires driver's license item to buy any other license
- In-game notifications for all actions (localized)
- PED menu with NUI interface
- License expiry and renewal system


## Installation
1. Place the `tb_licenses` folder in your server's resources directory.
2. Add `ensure tb_licenses` to your `server.cfg`.
3. Make sure you have QBCore and its dependencies installed.
4. Configure the PED location and license types in `config.lua` as needed.

## Configuration
- **PED Location:**
  - Set in `config.lua` under `Config.Ped`.
  - Example:
    ```lua
    Config.Ped = {
        model = "a_m_m_skater_01",
        coords = vector3(-266.28, -967.53, 31.22),
        heading = 261.15,
        scenario = "WORLD_HUMAN_CLIPBOARD"
    }
    ```
- **Licenses:**
  - Add or edit license types in `Config.Licenses` in `config.lua`.
  - Each license has a label, type, item, price, expiry, etc.
- **Localization:**
  - Edit `Config.Lang` in `config.lua` for notification messages.

## Usage
- Approach the PED and press `E` to open the license menu.
- Click a license to purchase it (must have enough cash and, for non-driver licenses, a driver's license item).
- Expired licenses can be renewed from the menu.
- Police can use `/checklicenses [id]` to view a player's licenses.

## Requirements
- QBCore Framework
- qb-inventory (for item handling)
-

## Credits
- Script by TB SCRIPTS


## Support
For issues or suggestions, open an issue on the repository or contact the sc
