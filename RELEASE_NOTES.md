# Andy's Configurable Vein Miner and Tree Capacitor 2.2.1

Version 2.2.1 fixes the hosted-server operator menu so every toggle saves to its matching setting while preserving all existing mining behavior and all 72 settings.

## Fixed

- Fixed Ores reverting to off after saving through `/scriptevent andy_vmtc:config`.
- Fixed the remaining toggles being shifted to the wrong setting positions.
- Added strict response validation so malformed form data cannot alter the saved configuration.
- Kept existing 2.2.0 persistent server settings fully compatible.

Direct server-console commands continue to work normally. Mining speed, sounds, drops, durability, supported blocks, trees, leaves, gravity-block handling, and optional compatibility are unchanged.
