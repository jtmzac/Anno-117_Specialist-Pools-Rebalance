# Specialist Pools Rebalance
Update v1.1.0: The item pools have been refined more, mostly so you don't need to cross regions as much, see the v1.1 changes section for more details. Added options to re-add the common and/or rare productivity specialists, see the appropriate section for more details. Added fixes for all the productivity specialists that were missing or had wrong buildings in their buff target pools.

Overhauls the specialist pools for the four neutral traders Diana, Valeria, Procurator and Manx by removing low value specialists and categorising the rest based on the trader.

Each of the four traders now has a manually curated list of specialists taken from the combined pools of the neutral traders, pirates and rival npcs. This does not include the legendaries from research or from conquering/appointing other rival NPCs.

Valeria now has the civilian ship captains and The Procurator has all military specialists (captains and land buffs like towers and camps).

Diana and Manx provide nearly all the other specialists largely divided by region to minimise overlap and make it easier to get a specific specialist.

## What specialists have been Removed
The entire category of area buffs such as all bakeries in range of the specialist apply +1 fire safety to all buildings in range. These buffs mostly conflict with the main game design goal of spreading your production throughout a city and only really make sense for intermediate production zones. They're still very questionable value so have been entirely removed.

The common and rare productivity and maintenance specialists. There is an option to add back the common and/or rare productivity specialists, see the relevant section.
From my perspective these are quite low value due to the productivity bonus being only 10/20% and the maintenance bonuses only applying to the lowest tiers of workers. The issue with this is that buildings that use tier 1 and 2 workers tend to only use a few workers, so a -35% buff makes such a small difference that it doesn't seem worth it. The productivity bonuses are also heavily diluted because the game encourages you to use the massive bonuses from religion and aqueducts instead.

The city watch specialists have been removed as the limitation of only affecting their respective buildings within range of the villa/officium makes them nearly useless.

## What specialists remain
All captains and military land based specialists are still present but have been divided up between the Procurator and Valeria.

The epic tier productivity specialists have been kept as a 35% boost to productivity is quite notable.

Basic residence bonuses for the main seven attributes income/belief/knowledge/prestige/fire safety/health/happiness. These are simple but effective, even if you phase them out later in the game for more specialised buffs.

Residence buffs for providing specific needs. These are quite powerful and are good at encouraging providing all needs to all residences.

Some other smaller categories include aqueduct buffs, workforce buffs, and some public service building buffs.

All legendaries are still available and have been categorised accordingly.

# Who has what Specialist
The categorisation of specialists has been designed to make intuitive sense where possible with some small concessions between Diana and Manx to even the pools out a bit.

There is minimal overlap between traders. The main overlap is the money/knowledge/belief/prestige specialists are available at both Diana and Manx for convenience. The other is that Diana and Manx share most of their legendaries, except the small few that boost only their respective regions workforce. These are split accordingly.

## Valeria
Valeria now has all civilian ship captains with buffs like ship speed, cargo transfer speed, region transfer speed etc. She also has the basic residence buffs for fire safety/happiness/health.

## The Procurator
The Procurator now has all military ship captains with buffs to weapons or damage slowdown etc.

He also has all the land based military specialists that buff recruitment times, various tower buffs etc.

## Diana
Diana has all Latium goods based buffs along with the basic residence buffs for money/knowledge/belief/prestige.

## Manx
Manx has all Albion goods based buffs along with the basic residence buffs for money/knowledge/belief/prestige.

## Total Number of Specialists at each Trader
|Trader|Amount|+Common Prod|+Rare Prod|+CWSR|+RSaT|
|-----|-----|-----|
|Diana|62|13|5|0|0|
|Manx|63|10|12|0|0|
|Valeria|34|0|0|9|7|
|The Procurator|52|0|0|9|7|

CWSR = City Watch Specialist Rework
RSaT = Rival Specialists at Traders


# Adding the Common and/or Rare Productivity Specialists
To re-add one or both of these categories of specialists you need to find the "Include File" lines in assets.xml that should be around line 30.
Then uncomment the lines by removing the "<!--" from the start of the line and the "-->" from the end. This will allow them to be added back to the Diana and Manx pools.


# v1.1 Update Changes
Having played the game more with this mod, I wanted to refine the pools a bit more to improve convenience.

The remaining epic workforce/maintanence specialists removed, all workforce swap specialists removed. The former I don't think are practically useful, the latter are useless.

Diana/Manx now both have basic money/knowledge/belief/prestige specialists. You will probably want money and belief specialists in both regions and only having them in Latium was annoying.

Manx now also has Aqueduct/water consumption specialists instead of just Diana. This was missing since you still use a lot of aqueducts in Albion.

Fire safety/happiness/health specialists have been moved to Valeria. The chance of using these is fairly low so I moved them to the smallest item pool.

City Watch Specialist Rework now adds to Valeria and The Procurators pools instead of just Manx. Another convenience change.


# Extra Compatibility with City Watch Specialist Rework and/or Rival Specialists at Traders
If City Watch Specialist Rework is installed then the 9 city watch specialists will be automatically added back into both Valeria's and The Procurator's specialist pools.
If Rival Specialists at Traders is installed then the 7 rival npc specialists will be automatically added to both Valeria's and The Procurator's specialist pools.

Note that compatibility is based on the mod folder being installed and NOT what is activated in your active-profile.txt.


# Future Compatibility
This mod is not going to be useful in future unless it is manually updated with new specialists and probably new traders.

I spent hours identifying, extracting, categorising and then analysing and curating all these specialists manually and I cannot promise I will want to do that multiple times again in the future as updates and DLC is added.

If someone else wants to use this mod as a framework for doing the same thing with their own idea of balance you are more than welcome. I have left my internal lists that I used inside the mod files both for myself and anyone else who can benefit from them. For your own sanity, please use Visual Studio Code with the 117 mod plugin.

