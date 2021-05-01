# Useful links
https://forum.teknogods.com/viewtopic.php?t=38671
https://forum.teknogods.com/viewtopic.php?t=37793

# MW3 server commands
say [text]
kick [exact player name; not case sensitive]
map_rotate
start_map_rotate

start_map_rotate - starts the server
status - show player list with (name, xuid, hwid, ip)
dropclient/kickclient - kick player by client number, example: dropclient 5
drop/kick - kick player by name, example: kick "Unknown Soldier"
banclient - ban player by client number, example: banclient 5
ban - ban player by name, example: ban "Unknown Soldier"
killserver - shut down the server
map - change to the given map, example: map mp_dome
map_restart - restart the running map
fast_restart - same as above but the map is not re-loaded
quit - close the server
dumpuser - display detailed information about a player, example: dumpuser "Unknown Soldier"
loadScript - load an InfinityScript plugin, example: loadScript myPlugin.dll (myPlugin.dll must be present in the "scripts" folder) - takes effect after the next map restart
unloadScript - unload a previously loaded script, example: unloadScript myPlugin.dll - takes effect after the next map restart

# In game chat commands

commands.cs:
	already present commands of interest:
		say text (public)
		sayto player text (private)
		yell player text (private)
		ac130
		ua or unlimited_ammo <on/off/auto>
		tp player(to teleport) player(to teleport to)
		weapon <player | *filter*> <raw weapon string> [-t]
		MOAB disabled (commented out)

	//[my commands]
		ct - colour test (print chat message in all colours)
		dev - dev and rcon
		fl - toggle flying
		target - toggle being targeted by zombies
		takecurrent - remove current weapon
		takeall - remove all weapons
		nh - normal health (set health to 100)
		hh - set health to 5000 (jugg is )
		ih - infinite health (set health to 9999 every 50)
		money - 10,000 cash/score
		moremoney - 1,000,000 cash/score
		bigmoney - 1,000,000,000 cash/score

		ar - give autorevive
		pk - give all perks (includes +ar +gs +ew)

		emp
		sentry
		sentry2
		sentry3
		littlebird
		helisniper
		moab

		ew - enable weapon switching
		ga - max ammo
		gs - glowstick
		p1 - package 1 (pk, ew, ar, gs, bigmoney, hh, emp, sentry, littlebird, helisniper, moab)
		p2 - package 2 (za, dm, lg, usas, fmg9, ua on)

		dm - iw5_pecheneg_mp_rof_thermallmg;Death Machine
		tg - uav_strike_projectile_mp;Zeus Cannon
		za - stinger_mp;Zapper
		rg - iw5_skorpion_mp_eotechsmg_xmags_scope7;Porter's X2 Ray Gun
		nz - uav_strike_marker_mp;NZ75
		mk - iw5_mk12spr_mp_acog_xmags;MK12 SPR
		fmg9 - iw5_fmg9_mp_akimbo_xmags;Full Motion Glock 18
		lg - iw5_l96a1_mp_l96a1scopevz_xmags_camo11;L911C
		mg - iw5_mg36_mp_grip_xmags_camo11;Masseration Gun 72
		pecheneg - iw5_pecheneg_mp_thermal_xmags_camo11;PKP Pet-ur-egg
		usas - iw5_usas12_mp_reflex_xmags_camo11;USedASs-24
		1887 - iw5_1887_mp_camo11;Model 1337
	//[end my commands]



utilities.cs
	ua or unlimited ammo <on|off|auto> (works for sender only)
config.cs
	add command usage prompts
	add command messages/enabled/disabled



# Todo
- [ ] pa command - perfect aim
	- [ ] include in dm command
- [ ] Sort out left hand reload issue with !ia command
- [ ] Figure out perfect aim (like handgun crouching - no larger reticule when moving or shooting; use helisniper code - dm code doesnt allow ADS)
- [X] Make confirmation and error/usage messages for my commands
- [X] Make commands take player/filter arguments
	- [X] target
- [ ] What is dev command used for?
- [ ] Is oninterval enable weapon switch commands in pk command necessary?
- [ ] Does ew command need to be oninterval?
- [ ] Review commented out pa command
- [ ] Fix unlimited ammo breaks throwable killstreaks
	- [ ] make new ia (infinite ammo) command that targets specific players
	- [ ] make ia switch off-able
- [ ] Make money command which takes amount/value arguments
- [ ] Deconstruct latest AIZombies binary to find extra features
- [ ] Investigate InfinityScript reference functions in DGAdmin VS project
- [ ] Disable extraneous DGAdmin features to conserve script resource usage
	- [ ] isnipe mode

