# Prison Stash
Add to server/data/entitys.lua in mythic-inventiory.
```
	{
		id = 5000,
		slots = 15,
		capacity = 200,
		name = "Prison Stash",
	},
	{
		id = 5001,
		slots = 30,
		capacity = 200,
		name = "Public Prison Stash",
	},
```

Add to items/food/prison.lua in mythic-inventory.

```
{
		name = "fruitpunchslushie",
		label = "Prison Slushi",
		price = 5,
		isUsable = true,
		isRemoved = true,
		isStackable = 15,
		type = 1,
		rarity = 1,
		closeUi = true,
		weight = 0.5,
		isDestroyed = true,
		durability = (60 * 60 * 3),
		statusChange = {
			Add = {
				PLAYER_THIRST = 100,
			},
		},
		animConfig = {
			anim = "soda",
			time = 8000,
			pbConfig = {
				label = "Drinking",
				useWhileDead = false,
				canCancel = true,
				vehicle = false,
				disarm = true,
				ignoreModifier = true,
				disableMovement = false,
				disableCarMovement = false,
				disableMouse = false,
				disableCombat = true,
			},
		},
		metalic = false,
	},
	{
		name = "beatdownberryrazz",
		label = "Beatdown BerryRazz",
		price = 5,
		isUsable = true,
		isRemoved = true,
		isStackable = 15,
		type = 1,
		rarity = 1,
		closeUi = true,
		weight = 0.5,
		isDestroyed = true,
		durability = (60 * 60 * 3),
		statusChange = {
			Add = {
				PLAYER_THIRST = 50,
			},
		},
		animConfig = {
			anim = "soda",
			time = 8000,
			pbConfig = {
				label = "Drinking",
				useWhileDead = false,
				canCancel = true,
				vehicle = false,
				disarm = true,
				ignoreModifier = true,
				disableMovement = false,
				disableCarMovement = false,
				disableMouse = false,
				disableCombat = true,
			},
		},
		metalic = false,
		healthModifier = 25,
	},
```