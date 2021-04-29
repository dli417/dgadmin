# MW3 server commands



# In game chat commands

commands.cs:
	already present commands of interest:
		ac130
		unlimited_ammo <on/off/auto>
		weapon <player | *filter*> <raw weapon string> [-t]
		MOAB disabled (commented out)

	//[my commands]
		dev - dev and rcon
		fl - toggle flying
		target - toggle being targeted by zombies
		takecurrent - remove current weapon
		takeall - remove all weapons
		nh - normal health (set health to 100)
		hh - set health to 5000 (jugg is )
		ih - infinite health (set health to 9999 every 50)
		money - 10,000 cash/score
		bigmoney - 1,000,000,000 cash/score

		ar - give autorevive
		pk - give all perks (includes +ar +gs +ew)

		emp
		sentry
		littlebird
		helisniper
		moab

		ew - enable weapon switching
		pa - perfect aim (WIP)
		ga - max ammo
		gs - glowstick
		p1 - package 1 (pk, ew, ar, gs, bigmoney, hh, emp, sentry, littlebird, helisniper, moab)
		p2 - package 2 (za, dm, lg, usas, fmg9, ua on)

		dm - perfect later
		tg
		za - zapper
		rg
		nz - nz75
		mk
		fmg9
		lg - lg116
		mg
		pecheneg
		usas
		1887
	//[end my commands]



utilities.cs
	ua or unlimited ammo <on|off|auto> (works for sender only)
config.cs
	add command usage prompts
	add command messages/enabled/disabled



# Todo
- [ ] Sort out left hand reload issue with !ia command
- [ ] Figure out perfect aim (like handgun crouching - no larger reticule when moving or shooting; use helisniper code - dm code doesnt allow ADS)
- [ ] Make confirmation and error/usage messages for my commands
	- [X] ga - max ammo
	- [ ] dev - dev and rcon
	- [ ] fl - toggle flying
	- [ ] target - toggle being targeted by zombies
	- [ ] takecurrent - remove current weapon
	- [ ] takeall - remove all weapons
	- [ ] nh - normal health (set health to 100)
	- [ ] hh - set health to 5000 (jugg is )
	- [ ] ih - infinite health (set health to 9999 every 50)
	- [ ] money - 10,000 cash/score
	- [ ] bigmoney - 1,000,000,000 cash/score

	- [ ] ar - give autorevive
	- [ ] pk - give all perks (includes +ar +gs +ew)

	- [ ] emp
	- [ ] sentry
	- [ ] littlebird
	- [ ] helisniper
	- [ ] moab

	- [ ] ew - enable weapon switching
	- [ ] pa - perfect aim (WIP)
	- [ ] ga - max ammo
	- [ ] gs - glowstick
	- [ ] p1 - package 1 (pk, ew, ar, gs, bigmoney, hh, emp, sentry, littlebird, helisniper, moab)
	- [ ] p2 - package 2 (za, dm, lg, usas, fmg9, ua on)

	- [ ] dm - perfect later
	- [ ] tg
	- [ ] za - zapper
	- [ ] rg
	- [ ] nz - nz75
	- [ ] mk
	- [ ] fmg9
	- [ ] lg - lg116
	- [ ] mg
	- [ ] pecheneg
	- [ ] usas
	- [ ] 1887

