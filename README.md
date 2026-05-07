# NPC-pathfinding-system
A modular NPC pathfinding system for Roblox with four behaviour states.

## Features
- Four behaviour states (idle, chase, attack, return)
- Automatic state managment
- Configurable range, attack range, despawn range
- Clean Nearest player detection

## Instalation
Copy and drop the script into serverscriptservice.

## Usage
```
local config = {
Range = 50, 		
DespawnRange = 150,	 
AttackRange = 5,	 
}

local Npc = npcsystem.Create(workspace.Rig, config) 
Npc:Start()
```

## Configuration 
In a configuration table you can modify:

Range = 50, 		 -- Detection range in studs
DespawnRange = 150,	 -- Distance from spawn before returning
AttackRange = 5,	 -- Distance to trigger attack state

## States 
- Idle - stays in place
- chase - chases after the nearest player in range
- attack - attacks the player in attack range
- return - returns to it's spawn position 
