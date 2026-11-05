# deadpoint

hardcore open-world post-apocalyptic alpine survival game built on roblox.

## overview

**deadpoint** is an open-world survival game set in a frozen, mountainous wasteland. players must navigate severe hypothermia, hostile roadside infected hordes, power outages, and resource scarcity while exploring abandoned alpine settlements, quonset military shelters, and ruined infrastructure.

the project combines modular roblox luau gameplay systems, realistic lighting and terrain kinematics, physical electrical grid networks, and full weapon customization.

## core systems

### 1. survival kinematics (`SurvivalManager`)
- **metabolic vitals**: real-time tracking of hunger, thirst, blood levels, and stamina.
- **body temperature & hypothermia**: dynamic exposure model where wind chill, altitude, and blizzards cause rapid body cooling unless players seek insulated shelter, kindle campfires, or equip thermal clothing (such as parkas).
- **trauma & injury**: fall damage, bleeding debuffs, and sprint exhaustion.

### 2. electrical grid & structure power
- **circuit simulation**: realistic power distribution interconnecting fuel-fed generators, power switches, and distribution nodes (`PowerDevices`, `PowerCable`).
- **facility restoration**: wire electrical lines across abandoned structures to restore floodlights (`PoweredLight`), security blast doors, and workshop machinery.
- **load management**: circuits trip or dim when power draw exceeds generator output.

### 3. scavenging & looting loop
- **poi exploration**: scavenge ruined alpine watchtowers, abandoned gas stations, quonset military huts, and derelict hospital wings.
- **timed scavenge mechanics**: interactive proximity prompt containers (`[e]` interact) with dynamic loot respawn cycles and search durations (`scavenge time`).
- **food & hydration**: perishable rations, clean water canteens, and medical supplies.

### 4. gunsmith workbench & combat
- **weapon modifications**: modular firearm platform with tactical attachment slots (muzzle brakes, suppressors, optical scopes).
- **recoil & ballistics**: calibrated spread kinematics, physical bullet drop, and reload timings.
- **threat ecology**: roadside infected spawners with proximity aggro, herd flocking, and night-time aggression spikes.

### 5. world & interface
- **environmental atmosphere**: dense alpine fog, dynamic daylight cycle, volumetric blizzards, and custom terrain materials.
- **inventory management**: clean grid inventory with equipment slots, item inspection, and fast hotbar switching (`[tab] inventory`).
- **survivor factions**: neutral npc camps (`SurvivorNPCs`), trading hubs, and environmental lore notes.

## file architecture

- `deadpoint.rbxl`: complete roblox place file containing terrain, 3d assets, lighting presets, and all client/server scripts.
- `.gitignore`: roblox studio auto-backup and temp file exclusion rules.

## getting started

1. clone the repository:
   ```bash
   git clone https://github.com/nnickahh/deadpoint.git
   ```
2. open `deadpoint.rbxl` directly in [roblox studio](https://www.roblox.com/create).
3. test play in studio using **test > play** or press `f5` to run client and server simulation.

## license

all game assets, scripts, and place builds are proprietary and reserved.
