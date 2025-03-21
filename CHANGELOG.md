=============================CHANGES FOR ALL LEVELS (excluding intro) =============================

[DONE] Added health bar to HUD
-Changed ui\hud\masterchief.new_hud_definition->Bitmap Widgets[7] and ui\hud\dervish.new_hud_definition->Bitmap Widgets[7]:
 --Input 1: From BASIC Zero to UNIT Body
 --Unit flags -> motion sensor enabled: Uncheck
 --Flags->Flip Vertically: Checked
 --Bitmap: shield_meter
 --Shader: shield_test
 --Fullscreen Sequence Index: 0
 --Halfscreen Sequence Index: 2
 --Quarterscreen Sequence Index: 2
 --Fullscreen Offset Y: -38
 --Halfscreen Offset Y: -15
 --Quarterscreen Offset Y: -15

[DONE] Increased your movement speed
-Changed globals\globals.matg->Player Information->Run Forward: From 2.25 to 2.35
-Changed globals\globals.matg->Player Information->Run Backward: From 2 to 2.1
-Changed globals\globals.matg->Player Information->Run Sideways: From 2 to 2.1

[DONE] Increase player health
-Changed from 30 to 45

=============================CHANGES FOR ALL LEVELS (excluding intro and tutorial) =============================

[DONE] Reduced enemy damage multiplier and rate of fire
-Change globals\globals.matg->Difficulty->Heroic Rate of Fire: From 1.25 to 1
-Change globals\globals.matg->Difficulty->Impossible Rate of Fire: From 1.5 to 1

[DONE] Adjust delay for enemy melee attack
-Change globals\globals.matg->Difficulty->Hard Melee Delay Scale: From 0.4 to 0.7
-Change globals\globals.matg->Difficulty->Impossible Melee Delay Scale: From 0.1 to 0.4

[DONE] Increased your melee attack damage and have melee not hurt allies
-Changed globals\globals.matg->Damage Table->Damage Groups[3: Name="melee"]->Armor Modifiers[25: Name="tough_floodflesh"]: From 0.25 to 0.75
-Change objects\weapons\damage_effects\dash_melee.jpt!->Damage Lower Bound: From 150 to 175
-Change objects\weapons\damage_effects\dash_melee.jpt!->Damage Upper Bound min: From 150 to 175
-Change objects\weapons\damage_effects\dash_melee.jpt!->Damage Upper Bound max: From 150 to 175
-Change objects\weapons\damage_effects\slice_melee.jpt!->Flags->Does Not Hurt Friends: From unchecked to checked
-Change objects\weapons\damage_effects\smash_melee.jpt!->Flags->Does Not Hurt Friends: From unchecked to checked
-Change objects\weapons\damage_effects\smash_melee.jpt!->Damage Lower Bound: From 40 to 60
-Change objects\weapons\damage_effects\strike_melee.jpt!->Flags->Does Not Hurt Friends: From unchecked to checked
-Change objects\weapons\damage_effects\strike_melee.jpt!->Damage Lower Bound: From 20 to 45
-Change objects\weapons\damage_effects\strike_melee.jpt!->Damage Upper Bound min: From 60 to 90
-Change objects\weapons\damage_effects\strike_melee.jpt!->Damage Upper Bound max: From 60 to 90

[DONE] Adjust brute melee attack
-Change objects\weapons\damage_effects\brute_melee.jpt!->Damage Upper Bound min: From 35 to 30
-Change objects\weapons\damage_effects\brute_melee.jpt!->Damage Upper Bound max: From 40 to 35
-Change objects\characters\brute\damage_effects\brute_melee.jpt!->Instantaneous Acceleration: From 1.5 to 1.75

[DONE] Fixed heretic (w/carbine), Flood (w/energy sword), and AI (w/plasma rifle) melee attacks
-Changed ai\generic.char->Weapons Properties[29: Weapon="plasma_rifle"]->Weapon Melee Damage: From strike_melee to to null
-Change objects\characters\heretic\damage_effects\heretic_melee.jpt!->Damage Inner Cone Angle: From 15 to 90
-Change objects\characters\heretic\damage_effects\heretic_melee.jpt!->Damage Outer Cone Angle: From 30 to 115
-Change objects\characters\heretic\damage_effects\heretic_melee.jpt!->General Damage: From <blank> to melee
-Change objects\characters\floodcombat_human\damage_effects\floodcombat_human_charge_first_melee.jpt!->Damage Lower Bound: From 35 to 15
-Change objects\characters\floodcombat_human\damage_effects\floodcombat_human_charge_first_melee.jpt!->Damage Upper Bound min: From 35 to 20
-Change objects\characters\floodcombat_human\damage_effects\floodcombat_human_charge_first_melee.jpt!->Damage Upper Bound max: From 40 to 25
-Change objects\characters\floodcombat_human\damage_effects\floodcombat_human_charge_first_melee.jpt!->Damage Outer Cone Angle: From 50 to 60
-Change objects\characters\floodcombat_human\damage_effects\floodcombat_human_charge_first_melee.jpt!->Instantaneous Acceleration: From 1.5 to 1
-Change objects\characters\floodcombat_elite\damage_effects\floodcombat_human_charge_first_melee.jpt!->Damage Lower Bound: From 35 to 15
-Change objects\characters\floodcombat_elite\damage_effects\floodcombat_elite_charge_first_melee.jpt!->Damage Upper Bound min: From 35 to 20
-Change objects\characters\floodcombat_elite\damage_effects\floodcombat_elite_charge_first_melee.jpt!->Damage Upper Bound max: From 40 to 25
-Change objects\characters\floodcombat_elite\damage_effects\floodcombat_elite_charge_first_melee.jpt!->Damage Outer Cone Angle: From 50 to 60
-Change objects\characters\floodcombat_elite\damage_effects\floodcombat_elite_charge_first_melee.jpt!->Instantaneous Acceleration: From 1.5 to 1
-Change objects\weapons\damage_effects\ai_dash_melee.jpt!->Radius min: From 1 to 0.7
-Change objects\weapons\damage_effects\ai_dash_melee.jpt!->Radius max: From 1.3 to 1
-Change objects\weapons\damage_effects\ai_dash_melee.jpt!->Damage Upper Bound min: From 150 to 100
-Change objects\weapons\damage_effects\ai_dash_melee.jpt!->Damage Upper Bound max: From 150 to 100
-Change objects\weapons\damage_effects\ai_dash_melee.jpt!->Damage Outer Cone Angle: From 40 to 75
-Change objects\characters\elite\damage_effects\elite_melee.jpt!->Damage Lower Bound: From 20 to 45
-Change objects\characters\elite\damage_effects\elite_melee.jpt!->Damage Upper Bound min: From 35 to 75
-Change objects\characters\elite\damage_effects\elite_melee.jpt!->Damage Upper Bound max: From 35 to 75
-Change objects\characters\elite\damage_effects\elite_melee.jpt!->General Damage: From <blank> to melee

[DONE] Made it easier to assassinate enemies without alerting others
-Changed ai\generic.char->Perception Properties[*]->Non-Combat Perception Time: From 0/0.5/1/2 to 1.5

[DONE] Made Drones headshotable and slower
-Change objects\characters\bugger\ai\bugger.char->Normal Vitality: From 35 to 25
-Change objects\characters\bugger\ai\bugger.char->Legandary Vitality: From 45 to 35
-Change objects\characters\bugger\bugger.hlmt->Damage Sections[Name="head"]->Flags->Headshotable: From unchecked to checked
-Change objects\characters\bugger\bugger.hlmt->Targets[Marker Name="target_head"]->Flags->Headshot: From unchecked to checked
-Change objects\characters\bugger\bugger.hlmt->Targets[Marker Name="target_head"]->Flags->Headshot: From unchecked to checked
-Change objects\characters\bugger\bugger.biped->Flying->Max Velociy: From 5 to 4
-Change objects\characters\bugger\bugger.biped->Flying->Acceleration: From 18 to 12
-Change objects\characters\bugger\bugger.biped->Flying->Jump Velocity: From 2.1 to 1.4


[DONE] Decreased Flood Combat Form health (and make all Elite Combat Forms have shields)
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite.char->Character Stats->Health on easy: From 100 to 115
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite.char->Character Stats->Health on legendary: From 200 to 165
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite_shielded.char->Character Stats->Health on legendary: From 200 to 130
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite_shielded.char->Character Stats->Shields on easy: From 70 to 20
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite_shielded.char->Character Stats->Shields on legendary: From 100 to 40

[DONE] Decreased Brute health (and give all brutes helmets and have brute honor guard use captain as parent)
-Change objects\characters\brute\ai\brute.char->Character Stats->Health on easy: From 175 to 150
-Change objects\characters\brute\ai\brute.char->Character Stats->Health on legendary: From 250 to 175
-Change objects\characters\brute\ai\brute_captain.char->Character Stats->Health on easy: From 200 to 175
-Change objects\characters\brute\ai\brute_captain.char->Character Stats->Health on legendary: From 250 to 200
-Change objects\characters\brute\ai\brute_honor_guard.char->Parent Gunner: From brute_major to brute_captain
-Change objects\characters\brute\ai\brute_major.char->Character Stats->Health on legendary: From 200 to 175
-Change objects\characters\brute\brute.hlmt->Variants[0]->Regions[Name="helmet"]->Permutations->States[State="Destroyed"]->Initial Probability: From 0.5 to 0
-Change objects\characters\brute\brute.hlmt->Damage Sections[Name="helmet"]->Vitality Percentage: From 0.1 to 0.125

[DONE] Decreased gray sentinel shields and reduced emp radius
-Changed objects\characters\sentinel_aggressor\ai\sentinel_aggressor_major.char->Character Stats->Shields on normal: From 30 to 20
-Changed objects\characters\sentinel_aggressor\ai\sentinel_aggressor_major.char->Character Stats->Shields on legendary: From 60 to 30
-Change objects\characters\sentinel_aggressor\damage_effects\emp_death.jpt!->EMP Radius: From 5 to 3.5

[DONE] Make Plasma Grenade stick to weapons instead of bouncing off
-Change objects\weapons\grenade\plasma_grenade\plasma_grenade.proj->Material Responses[3]->Material Name: From hard_metal_thin_cov_hereticleader to hard_metal_thin
-Change objects\weapons\grenade\plasma_grenade\plasma_grenade.proj->Material Responses[3]->Global Material Index: From 62 to 54
-Change objects\weapons\grenade\plasma_grenade\plasma_grenade.proj->Material Responses[3]->Response: From Impact (Detonate) to Attach
-Change objects\weapons\grenade\plasma_grenade\plasma_grenade.proj->Material Responses[3]->Chance Fraction: From 0 to 1

[DONE] Adjust sniper damage
-Change sniper and beam rifle to 35 damage

[DONE] Added EMP to armed Plasma Grenade
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Radius min: From 0 to 0.25
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Radius max: From 0 to 1.5
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Side Effect: From None to EMP
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Area of Effect Core Radius: From 0 to 0.25
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Damage Lower Bound: From 400 to 25
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Damage Upper Bound min: From 400 to 200
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Damage Upper Bound max: From 400 to 200
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->EMP radius: From 0 to 0.25
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Radius min: From * to 0.25
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Radius max: From 1.5 to 1.75
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Side Effect: From None to EMP
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Damage Upper Bound min: From 120 to 200
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Damage Upper Bound max: From 120 to 200
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->EMP radius: From 0 to 0.25

[DONE] Increased chance of cascading chain-react grenade explosions
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_attached_explosion.jpt!->Category: From Plasma to Grenade
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_boarding_explosion.jpt!->Category: From Plasma to Grenade
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_equipment_explosion.jpt!->Radius max: From 1 to 1.5
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_equipment_explosion.jpt!->Category: From Plasma to Grenade
-Change objects\weapons\grenade\plasma_grenade\damage_effects\plasma_grenade_explosion.jpt!->Category: From Plasma to Grenade
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_equipment_explosion.jpt!->Radius min: From 0.5 to 0.75
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_equipment_explosion.jpt!->Radius max: From 1.25 to 1.5
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_equipment_explosion.jpt!->Area Of Core Radius: From 0.75 to 1
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_explosion.jpt!->Radius min: From 0.75 to 1
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_explosion.jpt!->Radius max: From 1.75 to 1.875
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_explosion.jpt!->Area Of Core Radius: From 0.75 to 1
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_explosion.jpt!->Damage Upper Bound min: From 150 to 165
-Change objects\weapons\grenade\frag_grenade\damage_effects\frag_grenade_explosion.jpt!->Damage Upper Bound max: From 150 to 165

[DONE] Increased chance marines and ultra grunts drop grenades
-Change objects\characters\marine\ai\marine.char->Grenade Properties[Grenade Type="Human Fragmentation"]->Don't Drop Grenades Chance: From 0.35 to 0.25
-Change objects\characters\grunt_ultra\ai\grunt_ultra.char->Grenade Properties[Grenade Type="Covenant Plasma"]->Don't Drop Grenades Chance: From 0.5 to 0.4

[DONE] Decrease change Jackals avoid grenades
-Change objects\characters\jackal\ai\jackal.char->Movement Properties->Dive Grenade Chance: From 0.5 to 0.25

[DONE] Increased time for AI (especially Jackals) to aim and fire Beam Rifle/Sniper Rifle
-Change objects\characters\jackal\jackal.bipd->Aiming Velocity Maximum: From 1200 to 600
-Change ai\generic.char->Weapons Properties[10: Weapon="beam_rifle"]->First Burst Delay Time: From 0.25 to 0.75
-Change ai\generic.char->Weapons Properties[26: Weapon="sniper_rifle"]->First Burst Delay Time: From 0.75 to 1.25
-Change ai\generic.char->Firing Pattern Properties[9: Weapon="beam_rifle"]->Firing Patterns[1]->Target Leading: From 1 to 0.875
-Change ai\generic.char->Firing Pattern Properties[9: Weapon="beam_rifle"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875

[DONE] Fixed Carbine rate of fire and reduced tracking
-Changed ai\generic.char->Firing Pattern Properties[21: Weapon="covenant_carbine"]->Firing Patterns[1]->Rate of Fire: From 6 to 5
-Changed ai\generic.char->Firing Pattern Properties[21: Weapon="covenant_carbine"]->Firing Patterns[1]->Target Leading: From 1 to 0.875
-Changed ai\generic.char->Firing Pattern Properties[21: Weapon="covenant_carbine"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875
-Changed objects\weapons\rifle\covenant_carbine\covenant_carbine.weap->Magazines->Rounds Reloaded: From 24 to 18
-Changed objects\weapons\rifle\covenant_carbine\covenant_carbine.weap->Barrels[0]->Fire Recovery Time: From 0.35 to 0.5
-Changed objects\weapons\rifle\covenant_carbine\covenant_carbine.weap->Barrels[1]->Fire Recovery Time: From 0.14 to 0.2

[DONE] Adjust AI tracking of battle rifle
-Changed ai\generic.char->Firing Pattern Properties[0: Weapon="battle_rifle"]->Firing Patterns[1]->Target Leading: From 1 to 0.875
-Changed ai\generic.char->Firing Pattern Properties[0: Weapon="battle_rifle"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875

[DONE] AI fires needler with longer delay between bursts
-Change [generic/elite]*.char->Firing Pattern Properties[23: Weapon="needler"]->Firing Patterns[*]->Burst Separation: Add 1
-Change [generic/elite]*.char->Firing Pattern Properties[23: Weapon="needler"]->Firing Patterns[*]->Burst Separation To: Add 1

[DONE] Decrease accuracy of Flood with plasma rifle and shotgun
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite*.char->Firing Pattern Properties[3: Weapon="shotgun"]->Firing Pattern[1]->Projectile Error: From 3 to 5
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite*.char->Firing Pattern Properties[9: Weapon="plasma_rifle"]->Firing Pattern[1]->Projectile Error: From 0 to 2

[DONE] Decreased Sentinel Beam depletion rate
-Changed objects\characters\sentinel_aggressor\weapons\beam\sentinel_aggressor_beam.weap->Misc->Age Generated Per Round: From 0.003 to 0.002
-Changed objects\characters\sentinel_aggressor\weapons\beam_elim\sent_agg_beam_elim.weap->Misc->Age Generated Per Round: From 0.0035 to 0.003

[DONE] Increased strength of Master Chief's flashlight
-Changed objects\characters\masterchief\flashlight_1p.ligh->Frustum Light->Cutoff Distance: From 6 to 10
-Changed objects\characters\masterchief\flashlight_3p.ligh->Frustum Light->Cutoff Distance: From 5 to 9

[DONE] Decreased Phantom turret health and have plasma grenades damage heavy vehicles
-Changed objects\vehicles\phantom\turrets\chin_gun\chin_gun.hlmt->New Damage Info->Maximum Vitality: From 100 to 60
-Changed objects\vehicles\phantom\turrets\side_gun\side_gun.hlmt->New Damage Info->Maximum Vitality: From 100 to 60
-Change globals\globals.matg->Damage Table->Damage Groups[20:Name="explosion_attached"]->Armor Modifiers[23:Name="hard_metal_thick"]->Damage Multiplier: From 0 to 0.3

[DONE] Reduced Heretic leader hologram damage
-Changed objects\characters\heretic\ai\heretic_leader_hologram.char->Firing Pattern Properties->Weapon Firing Assocations[*]->Weapon Damage Modifier: From 0.25/0.5 to 0.05

[DONE] Increased Plasma Pistol damage and its overcharge projectile speed (but reduced its homing)
-Changed ai\generic.char->Firing Pattern Properties[22:Weapon="plasma_pistol"]->Firing Patterns[1]->Rate of Fire: From 8 to 6
-Changed ai\generic.char->Firing Pattern Properties[22:Weapon="plasma_pistol"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875
-Changed ai\generic.char->Firing Pattern Properties[22:Weapon="plasma_pistol"]->Firing Patterns[1]->Target Leading: From 1 to 0.875
-Changed ai\floodcombat_elite\ai\floodcombat_elite.char->Firing Pattern Properties[10:Weapon="plasma_pistol"]->Firing Patterns[1]->Rate of Fire: From 10 to 8
-Change objects\weapons\pistol\plasma_pistol\projectiles\plasma_pistol_overcharged_bolt.proj->Initial Velocity: From 5 to 7
-Change objects\weapons\pistol\plasma_pistol\projectiles\plasma_pistol_charged_bolt.proj->Final Velocity: From 5 to 7
-Change objects\weapons\pistol\plasma_pistol\projectiles\plasma_pistol_charged_bolt.proj->Guided Angular Velocity Lower: From 80 to 30
-Change objects\weapons\pistol\plasma_pistol\projectiles\plasma_pistol_charged_bolt.proj->Guided Angular Velocity Upper: From 80 to 30
-Change globals\globals.matg->Damage Table->Damage Groups[1:Name="emp"]->Armor Modifiers[4:Name="energy"]->Damage Multiplier: From 0 to 100

[DONE] Increased time for AI to fire Rocket Launcher
-Changed ai\generic.char->Weapon Properties[15:Weapon="rocket_launcher"]->First Burst Delay Time min: From 0.5 to 1.5
-Changed ai\generic.char->Weapon Properties[15:Weapon="rocket_launcher"]->First Burst Delay Time max: From 1 to 1.5
-Changed characters\generic\ai\generic.char->Firing Pattern Properties[12:Weapon="rocket_launcher"]->Firing Patterns[*]->Burst Separation: * to 2.5
-Changed characters\generic\ai\generic.char->Firing Pattern Properties[12:Weapon="rocket_launcher"]->Firing Patterns[*]->Maximum Error Angle: From * to 0
-Changed characters\floodcombat_elite\ai\floodcombat_elite.char->Firing Pattern Properties[8:Weapon="rocket_launcher"]->Firing Patterns[*]->Burst Separation: * to 3
-Changed characters\floodcombat_elite\ai\floodcombat_elite.char->Firing Pattern Properties[8:Weapon="rocket_launcher"]->Firing Patterns[*]->Projectile Error: From * to 30

[DONE] Increased Flood Carrier Form speed, explosion damage, and number of infection forms
-Changed objects\characters\floodcarrier\floodcarrier.bidp->BIPED->Flags->Random Speed Increase: From unchecked to checked
-Changed objects\characters\floodcarrier\floodcarrier.bidp->Death Spawn Count: From 5 to 8
-Changed objects\characters\floodcombat_human\floodcombat_human.bipd->Death Spawn Character: From null to objects\characters\flood_infection\ai\flood_infection
-Changed objects\characters\floodcombat_human\floodcombat_human.bipd->Death Spawn Count: From 0 to 1
-Changed objects\characters\floodcarrier\damage_effects\suicide_explosion.jpt!->Area Of Effect Core Radius: From 0 to 0.75
-Changed objects\characters\floodcarrier\damage_effects\suicide_explosion.jpt!->Damage Upper Bound min: From 80 to 100
-Changed objects\characters\floodcarrier\damage_effects\suicide_explosion.jpt!->Damage Upper Bound max: From 80 to 100
-Changed objects\characters\floodcarrier\damage_effects\suicide_explosion.jpt!->Instantaneous Acceleration: From 2.75 to 3.75
-Changed objects\characters\flood_infection\damage_effects\infection_form_bite.jpt!->Damage Lower Bound: From 5 to 1
-Changed objects\characters\flood_infection\damage_effects\infection_form_bite.jpt!->Damage Upper Bound min: From 5 to 1
-Changed objects\characters\flood_infection\damage_effects\infection_form_bite.jpt!->Damage Upper Bound max: From 5 to 1
-Changed objects\characters\flood_infection\damage_effects\infection_form_pop.jpt!->Flags->Only Hurts One Infection Form: From checked to unchecked

[DONE] Slow turning rate of human combat forms
-Changed objects\characters\floodcombat_human\floodcombat_human.bidp->BIPED->Stationary Turning Threshold: From 90 to 75

[DONE] Decrease obstacle smash acceleration of flood combat forms
-Changed objects\characters\floodcombat_elite\floodcombat_elite_obstacle_smash.jpt!->Instantaneous Acceleration: From 2.5 to 2.25
-Changed objects\characters\floodcombat_human\floodcombat_human_obstacle_smash.jpt!->Instantaneous Acceleration: From 2.5 to 2.25

[DONE] Increased Plasma Turret rate of fire and damage against Flood
-Changed objects\weapons\c_turret_ap\weapon\big_needler.weap->Barrels->Rounds Per Second min: From 4 to 5
-Changed objects\weapons\c_turret_ap\weapon\big_needler.weap->Barrels->Rounds Per Second max: From 4 to 5
-Changed objects\vehicles\phantom\damage_effects\phantom_turret_bolt.jpt!->Specific Damage: From <empty> to kill_flood

[DONE] Increased Plasma Cannon projectile speed and damage to Flood
-Changed objects\weapons\fixed\plasma_cannon\projectiles\plasma_cannon_bolt.proj->Final Velocity: From 5 to 10
-Changed objects\weapons\fixed\plasma_cannon\damage_effects\plasma_cannon_bolt.jpt!->Specific Damage: From <empty> to kill_flood

[DONE] Increased Shadow speed, collision damage, and turret firing rate and allow it to be driven by player
-Changed objects\vehicles\creep\creep.vehi->Apply Collision Damage Scale: From 0.2 to 2
-Changed objects\vehicles\creep\creep.vehi->Maximum Forward Speed: From 2.25 to 3.1
-Changed objects\vehicles\creep\creep.vehi->Speed Acceleration: From 4.5 to 3
-Changed objects\vehicles\creep\creep.vehi->Speed Deceleration: From 0.45 to 1.5
-Changed objects\vehicles\creep\plasma_turret\weapons\creep_turret.weap->Barrels->Acceleration Time: From 4 to 2
-Changed objects\vehicles\creep\plasma_turret\weapons\creep_turret.weap->Barrels->Deceleration Time: From 4 to 2
-Changed objects\vehicles\creep\creep.vehi->Seats[0]->Flags->Invalid for Player: From checked to unchecked

[DONE] Increased Scorpion Tank speed and shell damage
-Changed objects\vehicles\scorpion\scorpion.vehi->Engine Max Angular Velocity: From 2 to 2.6
-Changed objects\vehicles\scorpion\damage_effects\shell_explosion.jpt!->Damage Upper Bound min: From 150 to 175
-Changed objects\vehicles\scorpion\damage_effects\shell_explosion.jpt!->Damage Upper Bound max: From 150 to 175
-Changed objects\vehicles\scorpion\damage_effects\shell_impact.jpt!->Damage Lower Bound: From 150 to 175
-Changed objects\vehicles\scorpion\damage_effects\shell_impact.jpt!->Damage Upper Bound min: From 150 to 175
-Changed objects\vehicles\scorpion\damage_effects\shell_impact.jpt!->Damage Upper Bound max: From 150 to 175

[DONE] Decreased Wraith mortar firing rate and increased damage
-Changed objects\vehicles\wraith\turrets\mortar\mortar_turret.weap->Barrels->Fire Recovery Time: From 1.1 to 1.25
-Changed objects\vehicles\wraith\damage_effects\wraith_mortar.jpt!->Area Of Effect Core Radius: From 1 to 1.25
-Changed objects\vehicles\wraith\damage_effects\wraith_mortar.jpt!->Damage Upper Bound min: From 200 to 225
-Changed objects\vehicles\wraith\damage_effects\wraith_mortar.jpt!->Damage Upper Bound max: From 200 to 225

[DONE] Increased Enforcer health and increased its mortar blast radius and grapple damage
-Changed objects\characters\sentinel_enforcer\ai\sentinel_enforcer.char->Health on easy: From 600 to 700
-Changed objects\characters\sentinel_enforcer\ai\sentinel_enforcer.char->Health on legendary: From 900 to 1000
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\grapple_melee.jpt!->Damage Lower Bound: From 200 to 300
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\grapple_melee.jpt!->Damage Upper Bound min: From 200 to 300
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\grapple_melee.jpt!->Damage Upper Bound max: From 200 to 300
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Radius min: From 0.75 to 1.25
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Radius max: From 2 to 2.25
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Damage Lower Bound: From 10 to 20
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Damage Upper Bound min: From 15 to 25
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Damage Upper Bound max: From 15 to 25
-Changed objects\characters\sentinel_enforcer\weapons\rocket\damage_effects\sentinel_enforcer_rocket_explosion.jpt!->Instantaneous Acceleration: From 0.4 to 0.6

[DONE] Adjust Enforcer movement to avoid getting stuck in doors
-Changed objects\vehicles\sentinel_enforcer\sentinel_enforcer.vehi->Speed Acceleration: From 8 to 6
-Changed objects\vehicles\sentinel_enforcer\sentinel_enforcer.vehi->Turn Rate: From 210 to 280

[DONE] Gave Elite Zealot same health/shield values as Elite Ultra
-Changed objects\characters\elite\ai\elite_zealot.char->Parent Gunner: From elite_major to elite_ultra

[DONE] Decreased Elite Ultra shield
-Changed objects\characters\elite\ai\elite_ultra.char->Character Stats->Shields on legendary: From 300 to 250

[DONE] Increased Banshee plasma bolt projectile speed (but reduced its tracking) and increased banshee bomb damage radius
-Changed objects\vehicles\banshee\weapon\banshee_bolt.proj->Initial Velocity: From 30 to 35
-Changed objects\vehicles\banshee\weapon\banshee_bolt.proj->Final Velocity: From 30 to 35
-Changed objects\vehicles\banshee\damage_effects\banshee_bomb_explosion.jpt!->Radius min: From 0.75 to 1
-Changed objects\vehicles\banshee\damage_effects\banshee_bomb_explosion.jpt!->Radius max: From 1.5 to 1.75
-Changed objects\vehicles\banshee\damage_effects\banshee_bomb_explosion.jpt!->Area Of Effect Core Radius: From 0.75 to 1
-Changed ai\generic.char->Firing Pattern Properties[6: Weapon="banshee_gun"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875
-Changed ai\generic.char->Firing Pattern Properties[6: Weapon="banshee_gun"]->Firing Patterns[1]->Target Leading: From 1 to 0.875

[DONE] Reduced Fuel Rod Gun rate of fire, and fix explosion damage
-Changed objects\weapons\support_high\flak_cannon\flak_cannon.weap->Barrels[0]->Fire Recovery Time: From 0.4 to 0.5
-Changed objects\weapons\support_high\flak_cannon\damage_effects\flak_explosion.jpt!->General Damage: From explosion_largw to explosion_large

[DONE] Increased SMG accuracy and dual-weilding damage
-Changed objects\weapons\rifle\smg\smg.weap->Angle Change: From * to 0
-Changed objects\weapons\rifle\smg\smg.weap->Projectile->Error Angle max: From 2.75 to 2.25
-Changed objects\weapons\rifle\smg\smg.weap->Dual Weapon Error->Dual Wield Damage Scale: From 0.75 to 0.875

[DONE] Increased Shotgun accuracy and range AI will fire it (but damage is reduced for AI)
-Changed objects\weapons\pistol\shotgun\damage_effects\shotgun_bullet.jpt!->Damage Lower Bound: From 5 to 2.5
-Changed objects\weapons\pistol\shotgun\damage_effects\shotgun_bullet.jpt!->Damage Upper Bound min: From 16.5 to 8.25
-Changed objects\weapons\pistol\shotgun\damage_effects\shotgun_bullet.jpt!->Damage Upper Bound max: From 16.5 to 8.25
-Changed objects\weapons\rifle\shotgun\shotgun.weap->Projectile->Projectile Per Shot: From 10 to 20
-Changed objects\weapons\rifle\shotgun\shotgun.weap->Projectile->Error Angle min: From 8 to 2.25
-Changed objects\weapons\rifle\shotgun\shotgun.weap->Projectile->Error Angle max: From 10 to 4.5
-Changed *.char->Firing Pattern Properties[1/3: Weapon="shotgun"]->Firing Patterns[*]->Weapon Damage Modifier: From 0 to 0.6

[DONE] Increased Magnum accuracy/damage/ammo
-Changed objects\weapons\pistol\magnum\magnum.weap->Projectile->Error Angle min: From 0.25 to 0
-Changed objects\weapons\pistol\magnum\magnum.weap->Projectile->Error Angle min: From 1.5 to 0.25
-Changed objects\weapons\pistol\magnum\magnum.weap->Magazines->Rounds Total Initial: From 36 to 84
-Changed objects\weapons\pistol\magnum\magnum.weap->Magazines->Rounds Total Maximum: From 60 to 96
-Changed objects\weapons\pistol\magnum\magnum.weap->Magazines->Runtime Rounds Inventory Maximum: From 48 to 84
-Changed objects\weapons\pistol\magnum\magnum.weap->Magazines->Magazine Equipment->Rounds: From 24 to 48
-Changed objects\weapons\pistol\magnum\damage_effects\magnum_bullet.weap->Damage Lower Bound: From 8 to 10
-Changed objects\weapons\pistol\magnum\damage_effects\magnum_bullet.weap->Damage Upper Bound min: From 8 to 10
-Changed objects\weapons\pistol\magnum\damage_effects\magnum_bullet.weap->Damage Upper Bound max: From 8 to 10
-Changed objects\weapons\pistol\magnum\damage_effects\magnum_bullet.weap->Specific Damage: From <blank> to kill_flood

[DONE] Increased body recharge fraction of marines
-Changed objects\characters\marine\ai\marine.char->Health on easy: From 100 to 120
-Changed objects\characters\marine\ai\marine.char->Health on legendary: From 150 to 170
-Changed objects\characters\marine\ai\marine.char->Body Recharge Fraction: From 0.5 to 0.75
-Changed objects\characters\marine\ai\marine_dress.char->Health on easy: From 130 to 150
-Changed objects\characters\marine\ai\marine_dress.char->Health on legendary: From 180 to 200
-Changed objects\characters\marine\ai\marine_dress.char->Body Recharge Fraction: From 0.5 to 1
-Changed objects\characters\marine\ai\marine_odst.char->Parent Character: From marine to marine_sgt
-Changed objects\characters\marine\ai\marine_sgt.char->Health on easy: From 130 to 150
-Changed objects\characters\marine\ai\marine_sgt.char->Health on legendary: From 180 to 200
-Changed objects\characters\marine\ai\marine_sgt.char->Body Recharge Fraction: From 0.5 to 1

[DONE] Increased chance marines evade grenades and avoid marines getting stuck on obstacles
-Changed objects\characters\marine\ai\marine.char->Movement Properties->Dive Grenade Chance: From 0.8 to 1
-Changed objects\characters\marine\ai\marine.char->Movement Properties->Flags->Hop (To Cover Path Segment): From unchecked to checked
-Changed objects\characters\marine\ai\marine.char->Movement Properties->Obstacle Leap Min Size: From None to Tiny
-Changed objects\characters\marine\ai\marine.char->Movement Properties->Obstacle Leap Max Size: From None to Tiny
-Changed objects\characters\marine\ai\marine.char->Evasion Properties[*]->Evasion Delay Timer: From 3/1.5/4.5 to 1.5

[DONE] Marines and ally Spec Ops Elites/Grunts only throw grenades if enemies are far enough away
-Changed objects\characters\marine\ai\marine.char->Grenade Properties[*]->Grenade Ranges min: From 2 to 3
-Changed objects\characters\marine\ai\marine.char->Grenade Properties[*]->Collateral Damage Radius: From 1.5 to 4
-Changed [Only on levels with Arbiter] objects\characters\elite\ai\elite_specops.char->Grenade Properties[*]->Grenade Ranges min: From 3 to 5
-Changed [Only on levels with Arbiter] objects\characters\elite\ai\elite_specops.char->Grenade Properties[*]->Collateral Damage Radius: From 2 to 6
-Changed [Only on levels with Arbiter and no Heretics] objects\characters\grunt\ai\grunt.char->Grenade Properties[*]->Grenade Ranges min: From 2 to 4
-Changed [Only on levels with Arbiter and no Heretics] objects\characters\grunt\ai\grunt.char->Grenade Properties[*]->Collateral Damage Radius: From 0 to 5
-Changed [Only on levels with Arbiter] objects\characters\grunt\ai\grunt_ultra.char->Grenade Properties[*]->Grenade Ranges min: From 2 to 4
-Changed [Only on levels with Arbiter] objects\characters\grunt\ai\grunt_ultra.char->Grenade Properties[*]->Collateral Damage Radius: From 0 to 5

[DONE] Decrease chance Elites melee on Flood levels
-Changed [The Oracle, Sacred Icon, and Quarantine Zone only] objects\characters\elite\ai\elite.char->Charge Properties[*]->Melee Chance: From * to 0.1

[DONE] Reduced Grunt Ultra plasma grenade use to uncover
-Changed objects\characters\grunt\ai\grunt_ultra.char->Grenade Properties->Grenade Throw Delay: From 1 to 2
-Changed objects\characters\grunt\ai\grunt_ultra.char->Grenade Properties->Grenade Uncover Chance: From 1 to 0.75

[DONE] Reduced Brute plasma grenade use and throwing distance
-Changed objects\characters\brute\ai\brute.char->Grenade Properties->Grenade Uncover Chance: From 0.4 to 0.2
-Changed objects\characters\brute\ai\brute.char->Grenade Properties->Anti-Vehicle Grenade Chance: From 0.4 to 0.2

[DONE] Increased Hunter health, reduced stun time, and adjusted melee hit box
-Changed objects\characters\hunter\ai\hunter.char->Character Stats->Health on easy: From 200 to 225
-Changed objects\characters\hunter\ai\hunter.char->Character Stats->Health on legendary: From 400 to 450
-Changed objects\characters\hunter\ai\hunter.char->Character Stats->Stun Time Bounds: From 2 to 1.5
-Changed objects\characters\hunter\ai\hunter.char->Character Stats->Stun Time Bounds To: From 3 to 1.75
-Changed objects\characters\hunter\damage_effects\hunter_charge_first_melee.jpt!->Radius min: From 1.25 to 0.75
-Changed objects\characters\hunter\damage_effects\hunter_charge_first_melee.jpt!->Radius max: From 1.5 to 1.25
-Changed objects\characters\hunter\damage_effects\hunter_charge_first_melee.jpt!->Damage Outer Cone Angle: From 50 to 65
-Change globals\globals.matg->Damage Table->Damage Groups[4:Name="sniper"]->Armor Modifiers[31:Name="soft_organic_flesh_hunter"]->Damage Multiplier: From 4 to 2

[DONE] Increased Plasma Rifle projectile speed and accuracy (but reduced tracking)
-Changed objects\weapons\rifle\plasma_rifle\projectiles\plasma_rifle_bolt.proj: Initial Velocity: From 14 to 20
-Changed objects\weapons\rifle\plasma_rifle\projectiles\plasma_rifle_bolt.proj: Final Velocity: From 14 to 20
-Changed ai\*.char->Firing Pattern Properties[27/9: Weapon="plasma_rifle"]->Firing Patterns[1]->Target Leading: From 1 to 0.875
-Changed ai\*.char->Firing Pattern Properties[27/9: Weapon="plasma_rifle"]->Firing Patterns[1]->Target Tracking: From 1 to 0.875

[DONE] Adjusted dual wielding damage penalty and accuracy for some weapons
-Changed objects\weapons\rifle\plasma_rifle\plasma_rifle.weap->Dual Weapon Error->Minimum Error: From 1 to 0.5
-Changed objects\weapons\rifle\plasma_rifle\plasma_rifle.weap->Dual Weapon Error->Error Angle min: From 1.5 to 1
-Changed objects\weapons\rifle\plasma_rifle\plasma_rifle.weap->Dual Weapon Error->Error Angle max: From 3 to 2.5
-Changed objects\weapons\rifle\brute_plasma_rifle\brute_plasma_rifle.weap->Dual Weapon Error->Dual Wield Damage Scale: From 0.75 to 0.875

[DONE] Increased Needler projectile speed (and increased tracking of Sentinel Enforcer needler)
-Changed objects\weapons\pistol\needler\projectiles\needler_shard\needler_shard.proj: Initial Velocity: From 6 to 7
-Changed objects\weapons\pistol\needler\projectiles\needler_shard\needler_shard.proj: Final Velocity: From 6 to 7
-Changed objects\characters\sentinel_aggressor\weapons\needler\sentinel_aggressor_needler_needle.proj: Initial Velocity: From 6 to 7
-Changed objects\characters\sentinel_aggressor\weapons\needler\sentinel_aggressor_needler_needle.proj: Final Velocity: From 6 to 7
-Changed objects\characters\sentinel_aggressor\weapons\needler\sentinel_aggressor_needler_needle.proj: Guided Angular Velocity Lower: From 5 to 15
-Changed objects\characters\sentinel_aggressor\weapons\needler\sentinel_aggressor_needler_needle.proj: Guided Angular Velocity Upper: From 10 to 20

[DONE] Increased AI firing duration of ghost gun
-Changed generic.char->Firing Pattern Properties[2: Weapon="ghost_gun"]->Firing Patterns[*]->Burst Duration: Add 0.25
-Changed generic.char->Firing Pattern Properties[2: Weapon="ghost_gun"]->Firing Patterns[*]->Burst Duration To: Add 0.25

[DONE] Have AI in ghost not take cover as fast
-Changed generic.char->Vehicle Properties[3: Unit="ghost"]->AI Cover Damage Threshold: From 0.2 to 0.8

[DONE] Increased AI firing duration of spectre plasma turret
-Changed generic.char->Firing Pattern Properties[37: Weapon="spectre\plasma_turret"]->Firing Patterns[*]->Burst Duration: From 1.5 to 2
-Changed generic.char->Firing Pattern Properties[37: Weapon="spectre\plasma_turret"]->Firing Patterns[*]->Burst Duration To: From 2 to 2.5

[DONE] Increased maximum AI firing distance for a few weapons
-Changed ai\generic->Weapon Properties[2: Weapon="smg"]->Maximum Firing Range: From 12 to 15

[DONE] Adjust plasma damage to energy
-Changed globals\globals.matg->Damage Table->Damage Groups[12: Name="plasma_slow"]->Armor Modifiers[4: Name="energy"]: From 1.5 to 1
-Changed globals\globals.matg->Damage Table->Damage Groups[14: Name="plasma_fast"]->Armor Modifiers[4: Name="energy"]: From 1 to 1.25

[DONE] Increased shields and delay of pistons and absorbers on Sacred Icon
-Changed scenerios\objects\solo\sentinelhq\door_piston_absorber\door_piston_absorber.hlmt->Maximum Shield Vitality: From 50 to 100
-Changed scenerios\objects\solo\sentinelhq\door_piston_absorber\door_piston_absorber.hlmt->Minimum Stun Damage: From 49 to 99
-Changed scenerios\objects\solo\sentinelhq\plug_absorber\plug_absorber.hlmt->Maximum Shield Vitality: From 50 to 100
-Changed scenerios\objects\solo\sentinelhq\plug_absorber\plug_absorber.hlmt->Minimum Stun Damage: From 49 to 99
-Changed scenerios\objects\solo\sentinelhq\door_piston\door_piston.mach->DEVICE->Delay Time: From 0.5 to 1.5
-Changed scenerios\objects\solo\sentinelhq\door_piston_top\door_piston_top.mach->DEVICE->Delay Time: From 0.5 to 1.5

[DONE] Decrease speed of large sentinel doors to avoid killing characters
-Changed scenerios\objects\solo\sentinelhq\door_sentinel\door_sentinel.mach->DEVICE->Position Transition Time: From 2 to 1
-Changed scenerios\objects\solo\sentinelhq\door_sentinel\door_sentinel.mach->DEVICE->Position Acceleration Time: From 4 to 12

[DONE] Enabled Wraith auto mini-turret and increased its accuracy
-Changed objects\vehicles\wraith\turrets\minigun\minigun.vehi->UNIT->Spawned Turrent Character: From ai\generic_turrent to ai\generic
-Changed objects\vehicles\wraith\turrets\minigun\minigun.vehi->Seats[0]->Built-in gunner: From ai\generic_turrent to ai\generic
-Changed ai\generic->Weapon Properties[use empty slot 35]: Copy values used by ai\generic_turret for minigun_turret
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Minimum Firing Range: From 0 to 2
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Maximum Firing Range: From 10 to 25
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Normal Combat Range: From * to 25
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Timid Combat Range: From * to 25
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Agressive Combat Range: From * to 25
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Normal Accuracy Bounds: From 0/0.4 to 0.4/0.6
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Normal Accuracy Time: From 20 to 8
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Heroic Accuracy Bounds: From 0.2/0.6 to 0.6/0.8
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Heroic Accuracy Time: From 14 to 6
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Legendary Accuracy Bounds: From 0.4/0.8 to 0.8/1
-Changed ai\generic->Weapon Properties[35: Weapon="minigun_turret"]->Legendary Accuracy Time: From 8 to 4
-Changed ai\generic->Firing Pattern Properties[any empty slot 35]:  Copy values used by ai\generic_turret for minigun_turret
-Changed ai\generic->Vehicle Properties[any empty slot 1]:  Copy values used by ai\generic_turret for minigun_turret

[DONE] Make stealth Elite fix to not climb in mid-air:
-Changed objects\characters\elite\ai\elite_stealth.styl->Special Movement->Climb: From checked to unchecked

[DONE] Prophet of Regret's Gravity Throne moves slower
-Changed objects\vehicles\gravity_throne\gravity_throne.vehi->Speed Acceleration: From 7.5 to 3.5

[DONE] Have Zealot wear correct helmet
-Changed objects\characters\elite\ai\elite_zealot.char->Variation->Name: From zealot_dog to zealot_scl
-Changed objects\characters\elite\ai\elite_zealot.char->Variation->Index: From -1 to 4
-Changed objects\characters\elite\ai\elite_zealot.char->Variation->Designator: From <blank> to scl

[DONE] Ensure Tartars' hammer does impact damage
-Changed effects\objects\characters\brute\tartarus_hammer_impact.effe->Locations[0]->MARKER NAMES: From melee_effect to up
-Changed objects\characters\brute\damage_effects\tartarus_hammer_melee.jpt!->Area Of Core Effect: From 0 to 1
-Changed objects\characters\brute\damage_effects\tartarus_hammer_melee.jpt!->Damage Lower Bound: From 150 to 250
-Changed objects\characters\brute\damage_effects\tartarus_hammer_melee.jpt!->Inner Cone Angle: From 20 to 10
-Changed objects\characters\brute\damage_effects\tartarus_hammer_melee.jpt!->Outer Cone Angle: From 40 to 50
-Changed objects\characters\brute\damage_effects\tartarus_hammer_melee.jpt!->Instant Acceleration: From 4 to 8
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Radius->min: From 0.4 to 0.8
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Radius->max: From 0.8 to 1.6
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Area Of Core Effect: From 0.8
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Damage Lower Bound: From 100 to 50
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Damage Upper Bound max: From 200 to 500
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Damage Upper Bound max: From 200 to 500
-Changed objects\characters\brute\damage_effects\tartarus_hammer_explosion.jpt!->Instant Acceleration: From 2 to 4

=============================SCENERIO CHANGES FOR ALL LEVELS=============================

[INCOMPLETE] Make all Elite Combat Forms have shields)
-Change scenerios\solo\*\*.scnr->Character Palette[Character="floodcombat_elite"]: From floodcombat_elite to floodcombat_elite_shielded

[INCOMPLETE] Decreased gray sentinel shields (and make all gray sentinels have shields) and reduced emp radius
-Change scenerios\solo\*\*.scnr->Character Palette[Character="sentinel_aggessor"]: From sentinel_aggessor* to sentinel_aggressor_major

=============================SCENERIO CHANGES FOR INDIVIDUAL LEVELS=============================

[DONE] ======CAIRO STATION======

[DONE] Replace a dual-weilding Elite ultra in last wave of the 2nd hanger bay with an ultra grunt with a needler
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Character Index: From 16 to 17
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Primary Weapon Index: From 5 to 4
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Secondary Weapon Index: From 5 to -1
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Location[0]->Character Index: From -1 to 16
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Location[0]->Primary Weapon Index: From -1 to 5
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[114: Name="bay2_cov_wv5_grt"]->Location[0]->Secondary Weapon Index: From -1 to 5

[DONE] Have enemies that ambush you at the exit of Habitat Delta initially be idle
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Orders[52: Name="atr1_cov_sec_back"]->Force Combat Status: Combat to Idle

[DONE] Have drones that ambush you at the elevator initially be idle
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads["elv_cov_floor_bgr"]->Legendary Diffculty Count: 5 to 3

[DONE] Increase number of enemies in a few places
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[22: Name="atr2_cov_floor_grt"]->Legendary Diffculty Count: From 2 to 3
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[26: Name="atr2_cov_lstair_grt"]->Legendary Diffculty Count: From 1 to 3
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[31: Name="atr2_cov_re_floor_grt"]->Legendary Diffculty Count: From 2 to 3
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[81: Name="trm1_cov_alock_elt"]->Legendary Diffculty Count: From 1 to 2
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[82: Name="trm1_cov_alock_grt"]->Legendary Diffculty Count: From 3 to 4
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[83: Name="trm1_cov_block_elt"]->Legendary Diffculty Count: From 1 to 3
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[84: Name="trm1_cov_block_grt"]->Legendary Diffculty Count: From 3 to 4
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->Squads[86: Name="dck_cov_arm1_elt"]->Legendary Diffculty Count: From 1 to 2
-Changed scenerios\solo\01b_spacestation\01b_spacestation.scnr->AI Trigger[32: dck_cov_back_fallback]->Condition[0]->X: From 2 to 1

[DONE] ======OUTSKIRTS======

[DONE] Made the randomly arriving Jackal snipers on Outskirts spawn at only two possible locations
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[1]->Position x: From * to -588.2995
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[1]->Position y: From * to -624.7553
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[1]->Position z: From * to 3.545623
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[1]->Facing y: From * to 0
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[3 and 4]->Position x: From * to -564.6778
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[3 and 4]->Position y: From * to -616.7495
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[3 and 4]->Position z: From * to 9.400217
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[25: Name="e1_cov_snipers0"]->Starting Locations[3 and 4]->Facing y: From * to 90.55318

[DONE] Increase number of enemies in a few places
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[8: Name="e1_cov_inf0_3"]->Legendary Diffculty Count: From 2 to 3
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[61: Name="e6_cov_inf0_0"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[69: Name="e8_cov_inf0"]->Legendary Diffculty Count: From 2 to 3
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[88: Name="e10_cov_inf1"]->Legendary Diffculty Count: From 2 to 3
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[98: Name="e11_cov_inf2"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[98: Name="e11_cov_inf2"]->Starting Locations[1]->Character Index: From -1 to 0
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[98: Name="e11_cov_inf2"]->Starting Locations[1]->Primary Weapon Index: From -1 to 1
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[98: Name="e11_cov_inf2"]->Starting Locations[1]->Seat Type: From No Driver to Driver
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[114: Name="e12_cov_ghosts0"]->Major Upgrade: From Normal to All

[DONE] Make stealth Elite that ambushes during sniper ally not dual wield:
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[45: Name="e4_cov_inf2"]->Starting Locations[0]->Always Place: From unchecked to checked
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[45: Name="e4_cov_inf2"]->Starting Locations[2]->Secondary Weapon Index: From 1 to -1
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[45: Name="e4_cov_inf2"]->Starting Locations[3]->Always Place: From unchecked to checked

[DONE] Add drivers to the Ghosts carried by the Shadows
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[125: Name="e13_cov_ghosts0"]->Starting positions[*]->Seat Type: No Driver to Driver

[DONE] Have enemies dropped off by first Phantom not just stand around
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[24: Name="e1_cov_inf4_2"]->Initial Order: From 39 to 37
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Orders[39]->Order Endings->Next Order Index: From 40 to 37
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Orders[39]->Order Endings->Delay Time: From 0 to 20

[DONE] Increase number of drones on Outskirts (e1_cov_inf3_main)
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Script Expressions[17098]->Value: From (real) 5 [0,0,-96,64] to 8 [0,0,-32,64]
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Script Expressions[17124]->Value: From (int16) 2 to 3
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Script Expressions[17130]->Value: From (int16) 10 to 12

[DONE] Added Hunters at end of Outskirts
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[126: Name="e13_cov_ghosts1"]->Vehicle Index: From 2 to -1
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[126: Name="e13_cov_ghosts1"]->Starting Locations[0 and 1]->Character Index: 5
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[126: Name="e13_cov_ghosts1"]->Starting Locations[0 and 1]->Primary Weapon Index: 7
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[126: Name="e13_cov_ghosts1"]->Starting Locations[2]->Vehicle Index: 2
-Changed scenerios\solo\03a_oldmombasa\03a_oldmombasa.scnr->Squads[126: Name="e13_cov_ghosts1"]->Starting Locations[2]->Seat Type: Driver

======METROPOLIS====== /////// Start here...

[DONE] Have all enemies piloting banshees be lowest rank (except brutes, heretics, and banshees on Regret)
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[15: Name="e15_cov_banshees0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[23: Name="e16_cov_banshees0_0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[24: Name="e16_cov_banshees0_1"]->Major Upgrade: From * to None

[DONE] Have enemies driving wraiths be certain ranks
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[5: Name="e14_cov_wraiths0"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[5: Name="e14_cov_wraiths0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[17: Name="e16_cov_wraiths0_0"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[17: Name="e16_cov_wraiths0_0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[18: Name="e16_cov_wraiths0_1"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[18: Name="e16_cov_wraiths0_1"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[19: Name="e16_cov_wraiths1"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[19: Name="e16_cov_wraiths1"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[50: Name="e19_cov_wraiths0_0"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[50: Name="e19_cov_wraiths0_0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_0"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_0"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_1"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_1"]->Major Upgrade: From * to None
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_2"]->Character Type Index: From 0 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[Name="e21_cov_wraiths0_2"]->Major Upgrade: From * to None

[DONE] Replace the late arriving banshee behind you
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[15: Name="e15_cov_banshees0"]->Normal Difficulty Count: From 2 to 1
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[15: Name="e15_cov_banshees0"]->Legendary Difficulty Count: From 2 to 1
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[15: Name="e15_cov_banshees0"]->Starting Locations[0]->Flags->Always Place: From unchecked to checked

[DONE] Additional enemies in some places
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[3: Name="e14_cov_ghosts0_0"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[4: Name="e14_cov_ghosts0_1"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[20: Name="e16_cov_ghosts0_0"]->Legendary Difficulty Count: From 3 to 4
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[20: Name="e16_cov_ghosts0_0"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[21: Name="e16_cov_ghosts0_1"]->Legendary Difficulty Count: From 1 to 2
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[21: Name="e16_cov_ghosts0_1"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[22: Name="e16_cov_ghosts1"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[26: Name="e16_cov_inf0_1"]->Major Upgrade: From None to All
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[27: Name="e16_cov_inf0_2"]->Major Upgrade: From None to All
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[56: Name="e20_cov_ghosts0"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[65: Name="e21_cov_ghosts0_0"]->Major Upgrade: From Normal to All
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[84: Name="e23_cov_inf0_0"]->Legendary Difficulty Count: From 4 to 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[84: Name="e23_cov_inf0_0"]->Starting Location[3]->Character Index: From 2 to 10
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[84: Name="e23_cov_inf0_0"]->Starting Location[3]->Primary Weapon Index: From 0 to 9
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[84: Name="e23_cov_inf0_0"]->Starting Location[3]->Actor Variant: From <blank> to shieldless
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[87: Name="e23_cov_inf0_3"]->Major Upgrade: From None to Normal
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[87: Name="e23_cov_inf0_3"]->Starting Location[0]->Character Index: From 6 to 10
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[87: Name="e23_cov_inf0_3"]->Starting Location[0]->Primary Weapon Index: From -1 to 9
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[87: Name="e23_cov_inf0_3"]->Starting Location[0]->Actor Variant: From <blank> to shieldless
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[88: Name="e23_cov_inf0_4"]->Major Upgrade: From None to Normal

[INCOMPLETE] Additional enemies in some places
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[13960]->Value: From (real) 3 [0,0,64,64] to 4 [0,0,-128,64]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[8578]->Value: From (real) 6 [0,0,-64,64] to 8 [0,0,0,65]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[8608]->Value: From (real) 6 [0,0,-64,64] to 8 [0,0,0,65]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[8613]->Value: From (real) 3 [0,0,64,64]  to 4 [0,0,-128,64]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[8638]->Value: From (real) 6 [0,0,-64,64] to 8 [0,0,0,65]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[8662]->Value: From (real) 6 [0,0,-64,64] to 8 [0,0,0,65]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[13452]->Value: From (int16) 4 to 12
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[13476]->Value: From (int16) 4 to 12
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[13495]->Value: From (int16) 4 to 12
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[13361]->Value: From (real) 0 [0,0,0,0] to 1 [0,0,-128,63]
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[14077]->Value: From (int16) 1 to 2
-Changed scenerios\solo\03a_oldmombasa\03b_newmombasa.scnr->Script Expressions[14090]->Value: From (int16) 10 to 14

[DONE] More marines shoot at Scarab with sniper
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[78: Name="e23_mars_inf1"]->Starting Location[1]->Primary Weapon Index: From -1 to 4

[INCOMPLETE] Have Phantom that drops off 2nd wraith not stop so long
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Script Expressions[14809]: From (int16) 0 to (int16) 1

[DONE] Make stealth Elite that ambushes in tunnel not dual wield
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[32: Name="e17_cov_inf0_2"]->Starting Locations[0]->Primary Weapon Index: From 1 to 13
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[32: Name="e17_cov_inf0_2"]->Starting Locations[0]->Secondary Weapon Index: From 1 to -1

[INCOMPLETE] Have marines wait until you leave tunnel to continue
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Kill Trigger Volumes[101: Name="tv_e17_near_exit"]->Position z: -14.69403 to -14.29403

[DONE] Limited the extra Jackal Sniper waves never from behind
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[92: Name="e18_cov_inf2_1"]->Character Index: From 10 to -1
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[92: Name="e18_cov_inf2_1"]->Primary Weapon Index: From 9 to -1
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[92: Name="e18_cov_inf2_1"]->Starting Locations[0: Name="sniper0"]->Character Index: From -1 to 10
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[92: Name="e18_cov_inf2_1"]->Starting Locations[0: Name="sniper0"]->Primary Weapon Index: From -1 to 9

[INCOMPLETE] Limited the extra Jackal Sniper waves on Metropolis
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Script Expressions[12491]: From (int16) 8 to (int16) 6
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Script Expressions[12499]: From (int16) 12 to (int16) 7

[INCOMPLETE] Adds more ghosts to the city encounter
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[56: Name="e20_cov_ghosts0"]->Normal Difficulty Count: From 2 to 4
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[56: Name="e20_cov_ghosts0"]->Legendary Difficulty Count: From 2 to 4

[DONE] Make scarab ultra dual-weilding
-Changed scenerios\solo\03b_newmombasa\03b_newmombasa.scnr->Squads[89: Name="e23_cov_inf1_0"]->Starting Locations[0]->Secondary Weapon Index: From -1 to 1

THE ARBITER:

[INCOMPLETE] Have all enemies piloting banshees be lowest rank (except brutes, heretics, and banshees on Regret)
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[107: Name="dogfight_initial_enemies"]->Major Upgrade: From * to All
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[108: Name="dogfight_enemies"]->Major Upgrade: From * to All

[INCOMPLETE] Provided more variety of weapons used by heretics and show heretic leader as dual wielding
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[7: Name="rec_center_grunts_01"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[10: Name="rec_center_grunts_03"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[12: Name="rec_center_heretic_04"]->Primary Weapon Index: From 6 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[16: Name="rec_center_grunts_06"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[18: Name="rec_center_grunts_07"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[33: Name="hangar_rein_her_02L"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[34: Name="hangar_rein_her_02R"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[65: Name="first_hall_heretic_01"]->Primary Weapon Index: From 6 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[73: Name="underhangar_grunts_01"]->Locations[0]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[87: Name="heretic_leader_01"]->Secondary Weapon Index: From -1 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[88: Name="heretic_leader_02"]->Secondary Weapon Index: From -1 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[89: Name="heretic_leader_03"]->Secondary Weapon Index: From -1 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[92: Name="bottling_heretics_01"]->Locations[0]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[93: Name="bottling_grunts_01"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[101: Name="bottling_grunts_05"]->Locations[0 and 3]->Primary Weapon Index: From -1 to 2

[INCOMPLETE] Heretic major with sword
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Squads[62: Name="hangar_heretic_06C"]->Major Upgrade: From Normal to All

[INCOMPLETE] Add additional banshee to end of The Arbiter
-Changed scenerios\solo\04a_gasgiant\04a_gasgiant.scnr->Script Expressions[24309]: From (int16) 2 to (int16) 3

THE ORACLE:

[INCOMPLETE] Allies at beginning of The Oracle do not throw grenades
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[0-3]->Grenade Type: From Covenant Plasma to None

[INCOMPLETE] Have all enemies piloting banshees be lowest rank (except brutes, heretics, and banshees on Regret)
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[96: Name="dogfighters_init"]->Major Upgrade: From * to All
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[97: Name="dogfighters_finale"]->Major Upgrade: From * to All

[INCOMPLETE] Provided more variety of weapons used by heretics and show heretic leader as dual wielding
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[35: Name="lab_heretics_above"]->Locations[0,2]->Primary Weapon Index: From -1 to 3
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[51: Name="bridge_heretics_final"]->Location[5]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[73: Name="control_return_heretics_02"]->Location[0]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[73: Name="control_return_heretics_02"]->Location[1]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[75: Name="control_return_heretics_03"]->Location[4]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[86: Name="power_core_heretics_01"]->Location[0]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[92: Name="heretic_leader_04"]->Secondary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[114: Name="underhangar_heretics_01"]->Location[0]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[114: Name="underhangar_heretics_01"]->Location[2]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[118: Name="underhangar_heretics_03"]->Location[0]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[118: Name="underhangar_heretics_03"]->Location[2]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[119: Name="underhangar_h_grunts_03"]->Location[0]->Primary Weapon Index: From -1 to 2
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[128: Name="heretic_leader_hangar"]->Secondary Weapon Index: From -1 to 0
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[148: Name="power_core_swords"]->Primary Weapon Index: From 4 to 0

[INCOMPLETE] More enemies at start of elevator
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8440]: From (int16) 2 to (int16) 4
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8444]: From (int16) 4 to (int16) 6

[INCOMPLETE] Speed up elevator
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[6741]: From (int16) 270 [14,1] to (int16) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[6783]: From (int16) 270 [14,1] to (int16) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[6825]: From (int16) 270 [14,1] to (int16) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[6909]: From (int16) 270 [14,1] to (int16) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8011]: From (int32) 300 [44,1] to (int32) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8057]: From (int32) 300 [44,1] to (int32) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8103]: From (int32) 300 [44,1] to (int32) 60
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[8145]: From (int32) 300 [44,1] to (int32) 60

[INCOMPLETE] Have Flood lab fight go faster
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[10282]: From (int32) 2000 [-48,7] to (int32) 600 [88,2]
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[10296]: From (int32) 1800 [8,7] to (int32) 1350 [70,5]
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[10306]: From (int32) 3600 [16,14] to (int32) 300 [44,1]
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[10317]: From (int32) 1800 [8,7] to (int32) 300 [44,1]

[INCOMPLETE] Only two banshees during last banshee fight
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[21873]: From (int32) 97 to (int32) 96
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Script Expressions[21874]: From (int16) 3 to (int16) 0

[INCOMPLETE] Made Heretic Leader hide out of sight while speaking
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[135: Name="hl_boss_random"]->Starting Locations[*]->Position z: From 49 to 50
-Changed scenerios\solo\04b_floodlab\04b_floodlab.scnr->Squads[135: Name="hl_boss_random"]->Starting Locations[*]->Initial Movement Mode: From Default to Flying

DELTA HALO:

[INCOMPLETE] Added an additional ODST and magnum at start of Delta Halo
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[0: Name="allies_lz_ledge"]->Locations[0]->Primary Weapon: From 2 to -1
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[6989]: From (int16) 2 to (int16) 3
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[7003]: From (int16) 2 to (int16) 3
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[7021]: From (int16) 2 to (int16) 3
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Weapons[3]->Palette Index: From 1 to 10
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Weapons[3]->Rounds Left: From 80 to 96
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Weapons[3]->Rounds Loaded: From 20 to 12

[INCOMPLETE] Have all enemies piloting banshees be lowest rank (except brutes, heretics, and banshees on Regret)
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squads[62: Name="bridge_banshees"]->Major Upgrade: From * to None
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squads[63: Name="bridge_pelican_chasers"]->Major Upgrade: From * to None

[INCOMPLETE] Added extra allies with Warthog on Delta Halo
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[7562]: From (float32) 2 [0,0,0,64] to (float32) 4 [0,0,-128,64]
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[31: Name="allies_lz_pelican"]->Locations[4]->Always Place: From unchecked to checked
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[31: Name="allies_lz_pelican"]->Locations[4]->Primary Weapon Index: From 2 to 9

[INCOMPLETE] Have enemies driving wraiths be certain ranks
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squads[35: Name="bridge_farside_wraiths"]->Character Type Index: From 1 to 5
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squads[35: Name="bridge_farside_wraiths"]->Major Upgrade: From * to None

[INCOMPLETE] Added extra enemies on Delta Halo
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[11009]: From (int16) 3 to (int16) 2
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13681]: From (int16) 4 to (int16) 7
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13689]: From (int16) 3 to (int16) 5
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13697]: From (int16) 2 to (int16) 3
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13766]: From (int16) 1 to (int16) 2
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13850]: From (float) 1 [0,0,-128,63] to (float) 2 [0,0,0,64]
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[14418]: From (int16) 5 to (int16) 7
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[14395]: From (int16) 2 to (int16) 0
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[14781]: From (int16) 3 to (int16) 4
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[14785]: From (int16) 3 to (int16) 4
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[15004]: From (int16) 5 to (int16) 7
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[22283]: From (int32) 1 to (int32) 2
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[22774]: From (int16) 5 to (int16) 4

[INCOMPLETE] Have banshees show up before wraiths are destroyed on Delta Halo
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[62: Name="bridge_banshees"]->Locations[0]->Always Place: From unchecked to checked
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[62: Name="bridge_banshees"]->Locations[1]->Always Place: From unchecked to checked
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13088]: From (int16) 1 to (int16) 3
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13132]: From (int16) 1 to (int16) 2
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13214]: From (int16) 1 to (int16) 2
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Script Expressions[13238]: From (int16) 2 to (int16) 4

[INCOMPLETE] Remove the last group of drones in the Delta Halo grotto
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[172: Name="grotto_buggers_03"]->Character Index: From * to -1
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[172: Name="grotto_buggers_03"]->Primary Weapon Index: From * to -1

[INCOMPLETE] Make sure drones after Delta Halo grotto show up
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[186: Name="approach_elite_03"]->Character Index: From 1 to 9
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[186: Name="approach_elite_03"]->Primary Weapon Index: From 0 to 5
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[186: Name="approach_elite_03"]->Starting Locations[0]:->Actor Variant: From * to shieldless
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[187: Name="approach_grunts_01"]->Normal Difficulty Count: From 2 to 1
-Changed scenerios\solo\05a_deltaapproach\05a_deltaapproach.scnr->Squad[187: Name="approach_grunts_01"]->Legendary Difficulty Count: From 2 to 1

REGRET:

[INCOMPLETE] Made shotgun start on Regret
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Player Starting Profile[0]->Secondary Weapon: From smg to shotgun
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Player Starting Profile[0]->Secondary Weapon Rounds Loaded: From 60 to 12
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Player Starting Profile[0]->Secondary Weapon Rounds Total: From 200 to 48
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[0: Name="initial_allies"]->Starting Locations[2]->Always Place: From unchecked to checked

[INCOMPLETE] Have all enemies piloting banshees be lowest rank (except brutes, heretics, and banshees on Regret)
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[124: Name="gondola_02_banshees"]->Character Index: From 0 to 1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[124: Name="gondola_02_banshees"]->Major Upgrade: From * to None
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Orders[153: Name="gondola_02_banshees"]->Force Combat Status: From None to Alert

[INCOMPLETE] Increase delay between enemies at start of Regret
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Script Expressions[4332]: From (int16) 90 to (int16) 180 [-76,0]
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Script Expressions[4339]: From (int16) 90 to (int16) 150 [-106,0]
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Script Expressions[4386]: From (float) 4 [0,0,-128,64] to (float) 3 [0,0,64,64]
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[1: Name="tower1_elites_01"]->Major Upgrade: From Normal to Few
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[2: Name="tower1_elites_02"]->Major Upgrade: From Normal to Few

[INCOMPLETE] Adjust initial Jackal sniper spawns to not be within the building on the right
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[18: Name="bridge_jackals_06"]->Starting Locations[0]->Position x: From 7.872038 to 5.372038
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[18: Name="bridge_jackals_06"]->Starting Locations[0]->Position y: From -193.7201 to -191.7201
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[18: Name="bridge_jackals_06"]->Starting Locations[0]->Position z: From 18.60028 to 18.50028
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[18: Name="bridge_jackals_06"]->Starting Locations[0]->Facing y: From 89.8083 to 129.8083
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Orders[11: Name="tower_cluster_ranged_05"]->Primary Area Set[2]->Area Index: From 6 to 9
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Orders[12: Name="tower_cluster_ranged_06"]->Primary Area Set[*]->Area Index: From * to 0

[INCOMPLETE] Fix Phantom carrying Hunters colliding with building
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Scripting Data[0]->Point Sets[1: Name="bsp1_airspace"]->Points[3: Name="ph_01_2"]->Position z: From 26.32971 to 28.32971

[INCOMPLETE] Replaced several of the Jackal snipers in sunken chamber on Regret with Elite Honor Guards and fuel rod Grunts
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Normal Difficulty Count: From 1 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Legendary Difficulty Count: From 1 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Character Index: From 9 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Primary Weapon Index: From 4 to 12
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Locations[0]->Character Index: From -1 to 9
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Locations[0]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Locations[0]->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[68: Name="sunk_chamber_init_js_R02"]->Locations[1]->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Normal Difficulty Count: From 1 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Legendary Difficulty Count: From 1 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Character Index: From 9 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Primary Weapon Index: From 4 to 12
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Locations[0]->Character Index: From -1 to 9
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Locations[0]->Primary Weapon Index: From -1 to 4
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Locations[0]->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squad[72: Name="sunk_chamber_init_js_L02"]->Locations[1]->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[79: Name="sunk_chamber_js_L_01"]->Character Index: From 9 to 1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[79: Name="sunk_chamber_js_L_01"]->Primary Weapon Index: From 4 to 0
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[79: Name="sunk_chamber_js_L_01"]->Starting Locations[*]->Actor Variant: From shieldless to <empty>
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[79: Name="sunk_chamber_js_L_01"]->Starting Locations[1]->Primary Weapon Index: From -1 to 6
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Character Index: From 9 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Primary Weapon Index: From 4 to 12
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Starting Locations[0]->Character Index: From -1 to 1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Starting Locations[0]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[80: Name="sunk_chamber_js_L_02"]->Starting Locations[*]->Actor Variant: From shieldless to <empty>
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[81: Name="sunk_chamber_js_R_01"]->Character Index: From 9 to 1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[81: Name="sunk_chamber_js_R_01"]->Primary Weapon Index: From 4 to 0
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[81: Name="sunk_chamber_js_R_01"]->Starting Locations[*]->Actor Variant: From shieldless to <empty>
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[81: Name="sunk_chamber_js_R_01"]->Starting Locations[1]->Primary Weapon Index: From -1 to 6
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Character Index: From 9 to 2
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Primary Weapon Index: From 4 to 12
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Starting Locations[0]->Character Index: From -1 to 1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Starting Locations[0]->Primary Weapon Index: From -1 to 0
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[82: Name="sunk_chamber_js_R_02"]->Starting Locations[*]->Actor Variant: From shieldless to <empty>

[INCOMPLETE] Have Stealth Sword Elite enter second tunnel be a Stealth Major
-Changed scenarios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[95: Name="tunnel_02_elites_03"]->Major Upgrade: From Normal to All

[INCOMPLETE] All of Prophet of Regret's Elite Honor Guards have Energy Swords, and most of his Grunts are Ultras
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[133: Name="temple_hg_01L"]->Starting Locations[*]->Primary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[133: Name="temple_hg_01L"]->Starting Locations[*]->Secondary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[134: Name="temple_hg_01R"]->Starting Locations[*]->Primary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[134: Name="temple_hg_01R"]->Starting Locations[*]->Secondary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[135: Name="temple_hg_02L"]->Starting Locations[*]->Primary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[135: Name="temple_hg_02L"]->Starting Locations[*]->Secondary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[136: Name="temple_hg_02R"]->Starting Locations[*]->Primary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[136: Name="temple_hg_02R"]->Starting Locations[*]->Secondary Weapon Index: From * to -1
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[153: Name="honor_grunts_init_R"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[154: Name="honor_grunts_init_L"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[155: Name="honor_grunts_new_R"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\05b_deltatowers\05b_deltatowers.scnr->Squads[156: Name="honor_grunts_new_L"]->Major Upgrade: From Normal to Many

SACRED ICON:

[INCOMPLETE] Fix overloaded carbines
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Player Starting Profile[0]: Rounds Loaded: From 18 to 10
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Player Starting Profile[0]: Rounds Total: From 96 to 82
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[16]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[19]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[25]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[26]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[29]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[38]->Rounds Left: From 117 to 36
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Weapons[45]->Rounds Left: From 117 to 36

[INCOMPLETE] Change all human combat forms with energy swords to elite combat forms
-Changed scenerios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[85: Name="qz_initial_flood_bridge"]->Location[1]->Character Index: From 9 to 2
-Changed scenerios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[94: Name="qz_cov_def_flood_d"]->Location[4]->Character Index: From 9 to 2
-Changed scenerios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[96: Name="qz_cov_def_flood_f"]->Location[3]->Character Index: From 9 to 2

[INCOMPLETE] Disabled several Sentinel emitters to fix pacing on Sacred Icon
EMITTERS_TO_DISABLE = 6,23,25,26,32,33,37,41,42,45,46,47,54,56,60,64,66,67,75,81
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Vehicles[EMITTERS_TO_DISABLE]->Variant Name: From <blank> to destroyed
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Vehicles[EMITTERS_TO_DISABLE]->Flags->Dead: From unchecked to checked

[INCOMPLETE] Adjusted AI spawns on Sacred Icon to fix pacing and increase AI numbers
-Changed scenerios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[18593]: From (int16) 150 [-106,0,0,0] to (int16) 60
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[29: plugholder_inf]->Normal Difficulty Count: From 3 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[29: plugholder_inf]->Legendary Difficulty Count: From 3 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[30: plugholder_bk_flood_a]->Normal Difficulty Count: From 3 to 1
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[30: plugholder_bk_flood_a]->Legendary Difficulty Count: From 3 to 1
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[31: plugholder_bk_flood_b]->Normal Difficulty Count: From 3 to 1
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[31: plugholder_bk_flood_b]->Legendary Difficulty Count: From 3 to 1
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[32: plugholder_bk_infec_a]->Normal Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[32: plugholder_bk_infec_a]->Legendary Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[33: plugholder_bk_infec_b]->Normal Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[33: plugholder_bk_infec_b]->Legendary Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[34: plugholder_lower_hall_flood]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[39: hall_c_flood_mid]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[42: hall_c_flood_d]->Legendary Difficulty Count: From 6 to 10
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[43: hall_c_flood_e]->Legendary Difficulty Count: From 6 to 10
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[53: ledge_a_flood_ini]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[56: ledge_a_flood_d1]->Normal Difficulty Count: From 3 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[56: ledge_a_flood_d1]->Legendary Difficulty Count: From 3 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[57: ledge_a_flood_d2]->Legendary Difficulty Count: From 3 to 5
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[62: cond_b_flood_tube_a]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[62: cond_b_flood_tube_a]->Legendary Difficulty Count: From 4 to 8
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[63: cond_b_flood_a_ini_a]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[64: cond_b_flood_a_ini_b]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[65: cond_b_flood_a_ini_c]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[67: cond_b_flood_a]->Normal Difficulty Count: From 3 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[67: cond_b_flood_a]->Legendary Difficulty Count: From 3 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[68: cond_b_flood_b]->Normal Difficulty Count: From 3 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[68: cond_b_flood_b]->Legendary Difficulty Count: From 3 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[69: cond_b_flood_c]->Legendary Difficulty Count: From 3 to 5
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[71: cond_b_flood_b_ini]->Normal Difficulty Count: From 3 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[71: cond_b_flood_b_ini]->Legendary Difficulty Count: From 3 to 8
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[71: cond_b_flood_b_ini]->Starting Locations[1]->Primary Weapon Index: From 11 to 8
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[71: cond_b_flood_b_ini]->Starting Locations[7]->Primary Weapon Index: From 5 to 7
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[72: cond_b_flood_c_ini_a]->Starting Locations[1]->Primary Weapon Index: From 11 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19732]->Value: From (float) 0 [0,0,0,0] to 6 [0,0,-64,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19733]->Value: From (float) 4 [0,0,-128,64] to 6 [0,0,-64,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[73: cond_b_flood_c_ini_b]->Starting Locations[4]->Primary Weapon Index: From 6 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19744]->Value: From (float) 6 [0,0,-64,64] to 7 [0,0,-32,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19748]->Value: From (float) 0 [0,0,0,0] to 7 [0,0,-32,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19749]->Value: From (float) 4 [0,0,-128,64] to 7 [0,0,-32,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[81: ledge_c_infec_fr]->Normal Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[81: ledge_c_infec_fr]->Legendary Difficulty Count: From 1 to 0
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[83: qz_initial_flood_ini]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[83: qz_initial_flood_ini]->Starting Locations[0]->Primary Weapon Index: From 4 to 8
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[85: qz_initial_flood_bridge]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[85: qz_initial_flood_bridge]->Legendary Difficulty Count: From 2 to 6
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[86: qz_initial_flood_camp]->Normal Difficulty Count: From 5 to 7
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[86: qz_initial_flood_camp]->Legendary Difficulty Count: From 4 to 11
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Team: From Default to Player
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Parent Squad Index Group: From 24 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Character Index: From 3 to 14
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[87: qz_initial_flood_carrier_camp]->Primary Weapon Index: From -1 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[88: qz_initial_flood_cave]->Legendary Difficulty Count: From 3 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[89: qz_ini_ins_pods]->Normal Difficulty Count: From 4 to 5
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[89: qz_ini_ins_pods]->Legendary Difficulty Count: From 4 to 5
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[90: qz_cov_def_flood_ini]->Normal Difficulty Count: From 3 to 5
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[90: qz_cov_def_flood_ini]->Legendary Difficulty Count: From 3 to 7
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[91: qz_cov_def_flood_a]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[91: qz_cov_def_flood_a]->Legendary Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[92: qz_cov_def_flood_b]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[92: qz_cov_def_flood_b]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[93: qz_cov_def_flood_c]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[93: qz_cov_def_flood_c]->Legendary Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[93: qz_cov_def_flood_c]->Starting Location[2]->Primary Weapon Index: From 13 to -1
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[94: qz_cov_def_flood_d]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[94: qz_cov_def_flood_d]->Legendary Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[94: qz_cov_def_flood_d]->Starting Location[0]->Primary Weapon Index: From 13 to 7
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[95: qz_cov_def_flood_e]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[95: qz_cov_def_flood_e]->Legendary Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[96: qz_cov_def_flood_f]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[96: qz_cov_def_flood_f]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[97: qz_cov_def_flood_g]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[97: qz_cov_def_flood_g]->Legendary Difficulty Count: From 2 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[97: qz_cov_def_flood_g]->Starting Location[3]->Primary Weapon Index: From 13 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[98: qz_cov_def_carrier]->Normal Difficulty Count: From 3 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[98: qz_cov_def_carrier]->Legendary Difficulty Count: From 3 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[98: qz_cov_def_carrier]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[98: qz_cov_def_carrier]->Starting Locations[1]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[101: qz_ini_turrets]->Character Index: From -1 to 16
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[101: qz_ini_turrets]->Primary Weapon Index: From -1 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[101: qz_ini_turrets]->Starting Locations[*]->Seat Type: From No Driver to Driver
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[102: qz_camp_turrets]->Character Index: From -1 to 16
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[102: qz_camp_turrets]->Primary Weapon Index: From -1 to 3
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[102: qz_camp_turrets]->Starting Locations[*]->Seat Type: From No Driver to Driver

[INCOMPLETE] Speed up encounter at end of Sacred Icon and add extra allies
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[17901]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[17835]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[17967]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[18033]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[18092]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[18144]->Value: From (int16) 1 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[20124]->Value: From (float) 0 [0,0,0,0] to 2 [0,0,0,64]
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Script Expressions[19671]->Value: From (int16) 0 to 1

[INCOMPLETE] Replace climbing human forms with climbing elite forms
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[91: qz_cov_def_flood_a]->Starting Locations[*]->Character Index: From 9 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[92: qz_cov_def_flood_b]->Starting Locations[*]->Character Index: From * to 9 (except when weapon is 8)
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[93: qz_cov_def_flood_c]->Starting Locations[*]->Character Index: From 9 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[94: qz_cov_def_flood_d]->Starting Locations[*]->Character Index: From 9 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[95: qz_cov_def_flood_e]->Starting Locations[*]->Character Index: From 9 to 2
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[96: qz_cov_def_flood_f]->Starting Locations[*]->Character Index: From * to 9 (except when weapon is 8)
-Changed scenarios\solo\06a_sentinelwalls\06a_sentinelwalls.scnr->Squads[97: qz_cov_def_flood_g]->Starting Locations[*]->Character Index: From 9 to 2

QUARANTINE ZONE:

[INCOMPLETE] Added additional Elite SpecOps allies so Spectres can be full
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[7: qz_cov_def_spec_ops]->Normal Difficulty Count: From 4 to 5
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[7: qz_cov_def_spec_ops]->Legendary Difficulty Count: From 4 to 5
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[106: qz_ext_b_cov_spec_ops]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[106: qz_ext_b_cov_spec_ops]->Legendary Difficulty Count: From 2 to 4

[INCOMPLETE] Remove driver of scorpion carried by pelican
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[29: qz_ext_a_dam_human]->Starting Locations[1]->Seat Type: From Default to No Driver

[INCOMPLETE] Change all human combat forms with energy swords to elite combat forms
-Changed scenerios\solo\06b_floodzone\06b_floodzone.scnr->Squads[85: Name="gorge_flood_ini"]->Location[3]->Character Index: From 7 to 2
-Changed scenerios\solo\06b_floodzone\06b_floodzone.scnr->Squads[88: Name="factory2_flood_ini"]->Location[5]->Character Index: From 7 to 2
-Changed scenerios\solo\06b_floodzone\06b_floodzone.scnr->Squads[90: Name="factory2_flood_bk"]->Location[0]->Character Index: From 7 to 2
-Changed scenerios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: Name="qz_ext_b_ent_flood_tube_b"]->Location[2]->Character Index: From -1 to 2
-Changed scenerios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: Name="qz_ext_b_ent_flood_tube_b"]->Location[4]->Character Index: From -1 to 2

[INCOMPLETE] Avoid Enforcers getting stuck in doors
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[31: qz_ext_a_dam_enf_door]->Starting Locations[0]->Position y: From -65.04976 to -65.54976
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[31: qz_ext_a_dam_enf_door]->Starting Locations[1]->Position x: From 16.64733 to 15.64733
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[31: qz_ext_a_dam_enf_door]->Starting Locations[2]->Position x: From 20.89063 to 20.39063

[INCOMPLETE] Position Rocket Flood in predictable locations
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[42: qz_ext_a_flood_c2]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[42: qz_ext_a_flood_c2]->Starting Locations[0]->Vehicle Index: From -1 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[42: qz_ext_a_flood_c2]->Starting Locations[0]->Primary Weapon Index: From -1 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[43: qz_ext_a_flood_d]->Normal Difficulty Count: From 5 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[43: qz_ext_a_flood_d]->Legendary Difficulty Count: From 5 to 8
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[43: qz_ext_a_flood_d]->Starting Locations[6]->Primary Weapon Index: From 6 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[86: gorge_flood_bk_cave]->Legendary Difficulty Count: From 5 to 7
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[86: gorge_flood_bk_cave]->Starting Locations[6]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[92: factory2_flood_bk_tunnel]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[92: factory2_flood_bk_tunnel]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[120: qz_ext_b_ent_ghost_bk]->Starting Locations[0]->Primary Weapon Index: From 6 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[122: qz_ext_b_ent_flood_tube_a]->Normal Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[122: qz_ext_b_ent_flood_tube_a]->Legendary Difficulty Count: From 4 to 10
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[122: qz_ext_b_ent_flood_tube_a]->Primary Weapon Index: From 6 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: qz_ext_b_ent_flood_tube_b]->Normal Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: qz_ext_b_ent_flood_tube_b]->Legendary Difficulty Count: From 4 to 10
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: qz_ext_b_ent_flood_tube_b]->Primary Weapon Index: From 6 to 1

[INCOMPLETE] Adjust enemy counts in various places
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[10: qz_cov_def_sen_elim]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[10: qz_cov_def_sen_elim]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[12: veh_int_enf_a]->Legendary Difficulty Count: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[15: veh_int_sen_elim_ini]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[15: veh_int_sen_elim_ini]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[15: veh_int_sen_elim_ini]->Starting Locations[0,1,3,4]: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[16: veh_int_sen_elim_lt]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[17: veh_int_sen_elim_rt]->Legendary Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[7737]->Value: From (int16) 0 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[34: qz_ext_a_dam_flood_ini]->Normal Difficulty Count: From 5 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[34: qz_ext_a_dam_flood_ini]->Legendary Difficulty Count: From 3 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[35: qz_ext_a_dam_flood_cliff_a]->Normal Difficulty Count: From 5 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[35: qz_ext_a_dam_flood_cliff_a]->Legendary Difficulty Count: From 3 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[36: qz_ext_a_dam_flood_cliff_b]->Normal Difficulty Count: From 3 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[36: qz_ext_a_dam_flood_cliff_b]->Legendary Difficulty Count: From 3 to 9
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[41: qz_ext_a_flood_c]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[48: ext_a_sen_elim_bk]->Legendary Difficulty Count: From 4 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[56: fact_ent_enf]->Normal Difficulty Count: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[56: fact_ent_enf]->Legendary Difficulty Count: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[57: fact_ent_sen]->Normal Difficulty Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[57: fact_ent_sen]->Legendary Difficulty Count: From 2 to 6
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[4119]->Value 00 (LSB): From 3 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[4109]->Value 00 (LSB): From 10 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->AI Triggers[0: Name='done fighting']->Conditions[0]->A: From 4 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Orders[5: cov_follow_factory1]->Flags->Inhibit Vehicle Use: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[67: factory_1_sentinels_initial_mid]->Starting Locations[1]->Character Index: From -1 to 11
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[67: factory_1_sentinels_initial_mid]->Starting Locations[1]->Primary Weapon Index: From 2 to 8
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[82: gorge_enf]->Starting Locations[1]->Character Index: From -1 to 11
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[82: gorge_enf]->Starting Locations[1]->Primary Weapon Index: From -1 to 8
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[82: gorge_enf]->Starting Locations[2]->Character Index: From -1 to 8
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[82: gorge_enf]->Starting Locations[2]->Primary Weapon Index: From -1 to 10
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[83: gorge_sen]->Normal Difficulty Count: From 2 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[83: gorge_sen]->Legendary Difficulty Count: From 2 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[84: gorge_flood_bk]->Legendary Difficulty Count: From 6 to 8
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[88: factory2_flood_ini]->Parent Squad Group: From 46 to 45
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Normal Difficulty Count: From 2 to 3
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Legendary Difficulty Count: From 2 to 5
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Character Index: From 2 to 3
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Primary Weapon Index: From 0 to -1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Starting Locations[2,3,4,6]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Starting Locations[3,4,6]->Character Index: From * to -1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[89: factory2_flood_mid]->Starting Locations[3,4,6]->Primary Weapon Index: From * to -1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[98: qz_ext_b_fact_ghosts]->Legendary Difficulty Count: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[102: qz_ext_b_fact_flood]->Starting Locations[15]->Primary Weapon Index: From 11 to 5
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[118: qz_ext_b_ent_turrets]->Normal Difficulty Count: From 3 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[118: qz_ext_b_ent_turrets]->Legendary Difficulty Count: From 3 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[118: qz_ext_b_ent_turrets]->Starting Locations[2,3,4,6]->Flags->Always Place: From unchecked to checked
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[122: qz_ext_b_ent_flood_tube_a]->Starting Locations[0]->Primary Weapon Index: From 7 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[123: qz_ext_b_ent_flood_tube_b]->Starting Locations[3]->Primary Weapon Index: From 11 to 1
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[9223]->Value: From (int16) 0 to 2

[INCOMPLETE] Allow spec ops with commander to get aboard scorpion
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[8873]->Value 00 (LSB): From 107 to 108
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[13749]->Value 00 (LSB): From 1 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Orders[129: qz_ext_b_fact_flood]->Flags->Inhibit Vehicle Use: From unchecked to checked

[INCOMPLETE] Replace climbing human forms with climbing elite forms
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[40: qz_ext_a_flood_rocket]->Character Index: From 7 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[41: qz_ext_a_flood_c]->Character Index: From 7 to 2

[INCOMPLETE] Change starting weapons of Elite ally for gondola ride
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[131: e21_cov_inf0_0]->Starting Locations[1]->Primary Weapon Index: From 2 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[131: e21_cov_inf0_0]->Starting Locations[1]->Secondary Weapon Index: From 2 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[132: e21_cov_inf0_1]->Starting Locations[1]->Primary Weapon Index: From 0 to 9

[INCOMPLETE] Increase number of flood on gondola
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12556]->Value: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12579]->Value: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12606]->Value: From 1 to 2
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12645]->Value: From 8 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12659]->Value: From 8 to 0
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12823]->Value: From 8 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12836]->Value: From 8 to 20
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12850]->Value: From 8 to 20

-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12851]->Value: From 67 to 69
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12853]->Value: From 67 to 69
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Script Expressions[12907]->Value: From 67 to 69

[INCOMPLETE] Alter spawn locations so only carriers enter on the bottom while combat forms enter on top
-Changed Squads[134: e21_fld_inf0_1, 135: e21_fld_inf0_2, 138: e21_fld_inf1_1, and 139: e21_fld_inf1_2]

134:
character index: 2
primary weapon index: -1
--------------------------------------------
x,y,z,facing,character index,primary weapon index
--------------------------------------------
2.160045,-0.02758781,7.000244,90,-1,-1,cs_e21_fld_inf0_high_entry,262
2.178642,0.8068848,7.000244,90,-1,3,cs_e21_fld_inf0_high_entry,262
2.268203,0.02099617,7.000244,90,-1,9,cs_e21_fld_inf0_high_entry,262
2.25795,0.9244385,7.000244,90,-1,9,cs_e21_fld_inf0_high_entry,262
2.307152,0.0833741,7.000244,90,-1,5,cs_e21_fld_inf0_high_entry,262
-2.322914,-0.3475342,7.000244,-90,-1,4,cs_e21_fld_inf0_high_entry,262
-2.318851,1.184082,7.000244,-90,-1,9,cs_e21_fld_inf0_high_entry,262
-2.412033,-0.3391114,7.000244,-90,-1,9,cs_e21_fld_inf0_high_entry,262
-2.399975,1.167724,7.000244,-90,7,5,cs_e21_fld_inf0_high_entry,262
-2.395859,-0.3669434,7.000244,-90,7,4,cs_e21_fld_inf0_high_entry,262
-0.01297406,7.959793,-1.479584,0,3,-1,cs_e21_fld_inf0_low_entry,261

135:
character index: 2
primary weapon index: -1
--------------------------------------------
x,y,z,facing,character index,primary weapon index
--------------------------------------------
2.160045,-0.02758781,7.000244,90,-1,-1,cs_e21_fld_inf0_high_entry,262
2.178642,0.8068848,7.000244,90,-1,9,cs_e21_fld_inf0_high_entry,262
2.268203,0.02099617,7.000244,90,-1,9,cs_e21_fld_inf0_high_entry,262
2.25795,0.9244385,7.000244,90,7,4,cs_e21_fld_inf0_high_entry,262
2.307152,0.0833741,7.000244,90,7,4,cs_e21_fld_inf0_high_entry,262

138:
character index: 2
primary weapon index: -1
--------------------------------------------
x,y,z,facing,character index,primary weapon index
--------------------------------------------
2.160045,-0.02758781,7.000244,90,-1,-1,cs_e21_fld_inf1_high_entry,260
2.178642,0.8068848,7.000244,90,-1,3,cs_e21_fld_inf1_high_entry,260
2.268203,0.02099617,7.000244,90,-1,9,cs_e21_fld_inf1_high_entry,260
2.25795,0.9244385,7.000244,90,-1,9,cs_e21_fld_inf1_high_entry,260
2.307152,0.0833741,7.000244,90,-1,5,cs_e21_fld_inf1_high_entry,260
-2.322914,-0.3475342,7.000244,-90,-1,4,cs_e21_fld_inf1_high_entry,260
-2.318851,1.184082,7.000244,-90,-1,9,cs_e21_fld_inf1_high_entry,260
-2.412033,-0.3391114,7.000244,-90,-1,9,cs_e21_fld_inf1_high_entry,260
-2.399975,1.167724,7.000244,-90,7,5,cs_e21_fld_inf1_high_entry,260
-0.01297406,7.959793,-1.479584,0,3,-1,cs_e21_fld_inf1_low_entry,259

139:
character index: 2
primary weapon index: -1
--------------------------------------------
x,y,z,facing,character index,primary weapon index
--------------------------------------------
-2.322914,-0.3475342,7.000244,-90,-1,-1,cs_e21_fld_inf1_high_entry,260
-2.318851,1.184082,7.000244,-90,-1,9,cs_e21_fld_inf1_high_entry,260
-2.412033,-0.3391114,7.000244,-90,-1,9,cs_e21_fld_inf1_high_entry,260
-2.399975,1.167724,7.000244,-90,-1,5,cs_e21_fld_inf1_high_entry,260
-2.395859,-0.3669434,7.000244,-90,7,4,cs_e21_fld_inf1_high_entry,260
-2.375343,1.017578,7.000244,-90,7,3,cs_e21_fld_inf1_high_entry,260

[INCOMPLETE] Added infection forms at end of mission
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[162: e26_fld_infection_forms0]->Starting Locations[0 and 2]->Swarm Count: From 2 to 4
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[162: e26_fld_infection_forms0]->Starting Locations[1 and 3]->Swarm Count: From * to 12
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[162: e26_fld_infection_forms0]->Starting Locations[1 and 3]->Placement Script: From * to <blanks>
-Changed scenarios\solo\06b_floodzone\06b_floodzone.scnr->Squads[162: e26_fld_infection_forms0]->Starting Locations[1 and 3]->Placement Script: From * to -1

GRAVEMIND:

[INCOMPLETE] Master Chief and prisoners start Gravemind with full health and shields
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[*]->Starting Health Damage: From 1 to 0
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[*]->Starting Shield Damage: From 1 to 0

[INCOMPLETE] Fix overloaded carbines
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[4: Name="jail_b_a"]->Rounds Loaded: From 30 to 18
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[4: Name="jail_b_a"]->Rounds Total: From 150 to 36

[INCOMPLETE] Place carbine at start of level and needler has full ammo
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[0-1]->Primary Weapon: From * to Needler
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[0-1]->Rounds Loaded: From * to 30
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[0-1]->Rounds Total: From * to 120
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Weapons[1]->Palette Index: From 6 to 2
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Weapons[1]->Rounds Left: From * to 54
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Weapons[1]->Rounds Loaded: From * to 18
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Weapons[1]->Position x: From * to -216.5272
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Weapons[1]->Position y: From * to -136.5268
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Squads[20: council_grunt_ini]->Starting Locations[1]->Primary Weapon: From -1 to 6

[INCOMPLETE] Have mid-level jail always first 
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21680]->Value: From 2 to 1

[INCOMPLETE] Have two marines start with SMGs
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[3,6]->Primary Weapon: From * to SMG
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[3,6]->Rounds Loaded: From * to 60
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Player Starting Profile[3,6]->Rounds Total: From * to 180

[INCOMPLETE] Always renew marines
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21703]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21729]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21805]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21919]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[21999]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22059]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22131]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22227]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22334]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22436]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22472]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22520]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22586]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22634]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22682]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22742]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22776]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22844]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22887]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[23016]->Value: From 3 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[23067]->Value: From 3 to 5

[DONE] Made it easier to assassinate enemies without alerting others
-Changed ai\generic.char->Perception Properties[*]->Non-Combat Perception Time: From 0/0.5/1/2 to 1.5
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[75: Name="room_a_tube_fodder"]->Flags->Deaf: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[75: Name="room_a_tube_fodder"]->Normal Diffculty Count: From 4 to 3
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[75: Name="room_a_tube_fodder"]->Legendary Diffculty Count: From 4 to 3
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[75: Name="room_a_tube_fodder"]->Locations[2,3,5]->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[63: Name="jail_brutes_ini"]->Style Index: From 2 to 5 (brute_no_berserk)
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[85: Name="jail_a_brute"]->Flags->Deaf: From unchecked to checked

[INCOMPLETE] Adjusted Gravemind prison spawns and fixed dead enemies coming down lift
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[78: Name="jail_brutes_ini"]->Character Index: From 19 to 20
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[78: Name="jail_brutes_ini"]->Starting Locations[0]->Position x: From -179.4852 to -179.7852
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[78: Name="jail_brutes_ini"]->Starting Locations[0]->Position y: From -137.147 to -137.047
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[78: Name="jail_brutes_ini"]->Starting Locations[1]->Position x: From -181.5179 to -181.2179
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[78: Name="jail_brutes_ini"]->Starting Locations[1]->Position y: From -135.9757 to -136.0757
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[79: Name="jail_grunts_ini"]->Normal Difficulty Count: From 6 to 7
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[79: Name="jail_grunts_ini"]->Legendary Difficulty Count: From 6 to 7
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[79: Name="jail_grunts_ini"]->Starting Locations[0,1,2,3,5,6,7]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[79: Name="jail_grunts_ini"]->Character Index: From 13 to 14
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[79: Name="jail_grunts_ini"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[80: Name="jail_jackals_ini"]->Normal Difficulty Count: From 3 to 2
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[80: Name="jail_jackals_ini"]->Legendary Difficulty Count: From 3 to 2
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[80: Name="jail_jackals_ini"]->Starting Locations[3,4]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[81: Name="jail_brutes_down"]->Normal Difficulty Count: From 2 to 1
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[81: Name="jail_brutes_down"]->Legendary Difficulty Count: From 2 to 1
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[81: Name="jail_brutes_down"]->Initial Orders: From 63 to 70
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[81: Name="jail_brutes_down"]->Starting Locations[1]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[82: Name="jail_grunts_down"]->Normal Difficulty Count: From 4 to 2
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[82: Name="jail_grunts_down"]->Legendary Difficulty Count: From 4 to 2
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[82: Name="jail_grunts_down"]->Starting Locations[2,3]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[83: Name="jail_jackals_down"]->Normal Difficulty Count: From 2 to 1
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[83: Name="jail_jackals_down"]->Legendary Difficulty Count: From 2 to 1
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[83: Name="jail_jackals_down"]->Starting Locations[2]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[85: Name="jail_a_brute"]->Character Index: From 20 to 19
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[85: Name="jail_a_brute"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[88: Name="jail_b_brutes"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[90: Name="jail_guard_brute_cell_a"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[92: Name="jail_guard_brute_cell_b"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[94: Name="jail_brute_c"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[95: Name="jail_brute_d"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[96: Name="jail_brute_e"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[97: Name="jail_brute_f"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[98: Name="jail_brute_g"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[99: Name="jail_brute_i"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[100: Name="jail_brute_j"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[101: Name="jail_brute_k"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[102: Name="jail_brute_l"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[103: Name="jail_brute_m"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[89: Name="jail_b_grunts"]->Character Index: From 13 to 14
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[89: Name="jail_b_grunts"]->Major Upgrade: From Normal to None

[INCOMPLETE] Have drones that ambush you after prison and on mauseleum bridge initially focus on another enemy squad
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[119: Name="room_b_elites"]->Force Combat Status: Combat to Alert
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[120: Name="room_b_buggers"]->Force Combat Status: Combat to Idle
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[89: Name="maus_bridge_buggers_rein"]->Flags->Follow Squad: From unchecked to checked
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[89: Name="maus_bridge_buggers_rein"]->Force Combat Status: Combat to Idle
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[89: Name="maus_bridge_buggers_rein"]->Follow Squad Index: From -1 to 222
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Orders[89: Name="maus_bridge_buggers_rein"]->Follow Radius: From 0 to 5

[INCOMPLETE] Fixed lightbridges and increased number of enemies during 2nd lightbridge
-Changed scenarios\solo\highcharity\high_gardens_tram.phmo->Lift Properties[0]->Linear Motion->Center Max Velocity: From 2 to 5
-Changed scenarios\solo\highcharity\high_gardens_tram.phmo->Lift Properties[0]->Linear Motion->Axis Acceleration: From 0 to 50
-Changed scenarios\solo\highcharity\high_gardens_tram.phmo->Lift Properties[0]->Linear Motion->Axis Max Velocity: From 0 to 50
-Changed scenarios\solo\highcharity\high_gardens_tram.phmo->Lift Properties[0]->Linear Motion->Direction Acceleration: From 0 to 10
-Changed scenarios\solo\highcharity\high_gardens_tram.phmo->Lift Properties[0]->Linear Motion->Direction Max Velocity: From 0 to 5
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22373]->Value: From (real) 0 [0,0,0,0] to 2 [0,0,0,64]
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22392]->Value: From (real) 0 [0,0,0,0] to 3 [0,0,64,64]
-Changed scenarios\solo\07a_highcharity\07a_highcharity.scnr->Script Expressions[22393]->Value: From (real) 2 [0,0,0,64] to 3 [0,0,64,64]

[INCOMPLETE] Have rangers in indoor midtower not dual-weilding
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[175: Name="midtower_elites"]->Normal Difficulty Count: From 3 to 4
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[175: Name="midtower_elites"]->Legendary Difficulty Count: From 3 to 4
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[175: Name="midtower_elites"]->Starting Locations[1,3]->Secondary Weapon Index: From 3 to -1

[INCOMPLETE] Have more brutes captains in mauseleum fight
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[233: Name="maus_inner_brutes_ini"]->Major Upgrade: From Normal to All
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[234: Name="maus_inner_brutes_rein"]->Normal Difficulty Count: From 3 to 4
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[234: Name="maus_inner_brutes_rein"]->Legendary Difficulty Count: From 3 to 6
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[234: Name="maus_inner_brutes_rein"]->Major Upgrade: From Normal to All

[INCOMPLETE] Have Zealot wear correct helmet
-Changed scenerios\solo\07a_highcharity\07a_highcharity.scnr->Squads[248: Name="maus_inner_elite_zealot"]->Starting Locations[*]->Actor Variant: From * to zealot_scl

UPRISING:

[INCOMPLETE] Change direction player is facing at start (Starting Positions and Cutscene Flags)
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Cutscene Flags[9: Name="player0_start"]->x Position: From  140.0429 to 140.5429
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Cutscene Flags[9: Name="player0_start"]->Facing Direction: From -176.151 to -136.151
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Cutscene Flags[10: Name="player1_start"]->x Position: From  140.2511 to 140.7511
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Cutscene Flags[10: Name="player1_start"]->Facing Direction: From -178.9248 to -138.9248

[INCOMPLETE] Have more variety in ally ranks of during the first half of mission and have them move from their starting locations
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[1: Name="e1_cov_inf1"]->Character Index: From 9 to 6
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[1: Name="e1_cov_inf1"]->Starting Locations[0]->Actor Variant: From spec_ops_dog to stealth_dog
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[2: Name="e1_cov_inf2"]->Major Upgrade: From None to Few
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[2: Name="e1_cov_inf2"]->Starting Location[1]->Character Index: From -1 to 9
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Orders[4: Name="e1_cov_inf_continue"]->Primary Area Set[0]: From Goal/0/11 to Goal/0/9
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[10: Name="e2_cov_inf0"]->Starting Locations[2]->Character Index: From 9 to 6
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[10: Name="e2_cov_inf0"]->Starting Locations[2]->Actor Variant: From * to stealth_dog
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Major Upgrade: From None to Many
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[36: Name="e6_cov_inf0"]->Normal Difficulty Count: From 2 to 4
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[36: Name="e6_cov_inf0"]->Legendary Difficulty Count: From 2 to 4
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[36: Name="e6_cov_inf0"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[37: Name="e6_cov_inf1"]->Starting Locations[1]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[70: Name="e10_cov_inf0"]->Major Upgrade: From None to Many
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[70: Name="e10_cov_inf0"]->Starting Location[1]->Primary Weapon Index: From -1 to 3

[INCOMPLETE] Have enemies driving wraiths be certain ranks
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[80: Name="e10_pro_wraith0_0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[81: Name="e10_pro_wraith0_1"]->Major Upgrade: From * to All

[INCOMPLETE] Change ai/generic.char to not attempt to ram ghost so much (Uprising only)
-Change ai/generic.char->Vehicle Assocations[3: ghost]->AI charge consider distance (0 to 4)
-Change ai/generic.char->Vehicle Assocations[3: ghost]->AI charge abort distance (0 to 4)

[INCOMPLETE] Adjust enemy spawns throughout the level
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[8: Name="e1_pro_inf0_3"]->Major Upgrade: From None to All
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[14: Name="e2_pro_inf0"]->Legendary Difficulty Count: From 4 to 5
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[21: Name="e3_pro_inf0_0"]->Legendary Difficulty Count: From 2 to 4
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[50: Name="e7_pro_inf0_1"]->Major Upgrade: From Normal to Few
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[51: Name="e7_pro_inf1_0"]->Major Upgrade: From Normal to Few
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[51: Name="e7_pro_inf1_0"]->Starting Locations[1]->Primary Weapon Index: From -1 to 3
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[52: Name="e7_pro_inf1_1"]->Major Upgrade: From Normal to Few
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[52: Name="e7_pro_inf1_1"]->Starting Locations[1]->Primary Weapon Index: From -1 to 3
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[54: Name="e7_pro_inf2"]->Starting Locations[*]->Flags->Initially Asleep: From unchecked to checked
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[59: Name="e8_pro_inf1_1"]->Starting Locations[1]->Flags->Character Index: From -1 to 2
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[59: Name="e8_pro_inf1_1"]->Starting Locations[1]->Flags->Primary Weapon Index: From 2 to 1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[59: Name="e8_pro_inf1_1"]->Starting Locations[2]->Flags->Primary Weapon Index: From 2 to -1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[75: Name="e10_pro_inf1_1"]->Starting Locations[1]->Primary Weapon Index: From -1 to 9
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[75: Name="e10_pro_inf1_1"]->Starting Locations[2]->Primary Weapon Index: From -1 to 9
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[76: Name="e10_pro_inf1_2"]->Legendary Difficulty Count: From 3 to 4
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[83: Name="e10_pro_ghosts0_0"]->Character Index: From 1 to 10
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[84: Name="e10_pro_ghosts0_1"]->Character Index: From 1 to 10

[INCOMPLETE] Help allies down the steps (on Uprising only)
-Changed objects\characters\elite\ai\elite.char->Movement Properties->Jump Height: From Stand to Storey

[INCOMPLETE] Adjust ally spawns throughout the level
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[55: Name="e8_cov_inf0"]->Starting Locations[4]->Character Type: From -1 to 0
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[55: Name="e8_cov_inf0"]->Starting Locations[4]->Primary Weapon: From -1 to 8
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[55: Name="e8_cov_inf0"]->Starting Locations[4]->Seat Type: From No Driver to Driver
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[55: Name="e8_cov_inf0"]->Initial Movement Distance: From 0 to 15
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[62: Name="e9_cov_ghosts0"]->Starting Locations[3]->Position x: From 284.9833 to 265.3703
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[62: Name="e9_cov_ghosts0"]->Starting Locations[3]->Position y: From 65.4101 to 97.73444
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[62: Name="e9_cov_ghosts0"]->Starting Locations[3]->Position z: From 32.26873 to 51.10955
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[62: Name="e9_cov_ghosts0"]->Starting Locations[3]->Facing y: From -3.735759 to 19.47164
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[62: Name="e9_cov_ghosts0"]->Starting Locations[3]->Vehicle Index: From -1 to 4
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[6946]->Value: From (float) 1 [0,0,-128,63] to 5 [0,0,-96,64]
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[6947]->Value: From (float) 3 [0,0,64,64] to 5 [0,0,-96,64]
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Starting Locations[2]->Character Index: From 5 to -1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Starting Locations[2]->Primary Weapon Index: From 1 to -1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Starting Locations[3,4]->Character Index: From 5 to 9
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Starting Locations[3]->Primary Weapon Index: From 1 to 3
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Squads[24: Name="e4_cov_inf0"]->Starting Locations[4]->Primary Weapon Index: From 1 to -1

[INCOMPLETE] Allow allies to get in vehicles right away
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[6187]->Value: From (int32) 19 to 21

[INCOMPLETE] Have brutes from armory not take so long
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[4042]->Value: From (int16) 2 to 1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[4055]->Value: From (int32) 450 [-62,1,0,0] to 150 [-106,0,0,0]

[INCOMPLETE] Change location of inserted pods and have them arrive earlier
-Changed scenarios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[4156]->Value: From 0 to 1
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Script Expressions[4051]->Value: From (int16) 34 to 31
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Scripts[97]: Change salt/index of e10_pod0_insertion[97] to that of e10_pod2_insertion[99]

[INCOMPLETE] Added more ammo to rocket launcher in armory
-Changed scenerios\solo\08a_deltacliffs\08a_deltacliffs.scnr->Weapons[0]->Rounds Left: From 2 to 4

HIGH CHARITY:

[INCOMPLETE] Adjust enemy spawns throughout the level
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squad Groups[6]->Parent: From 5 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squad Groups[7]->Parent: From 5 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[3: Name="e1_fld_inf1"]->Starting Locations[0]->Primary Weapon Index: From 1 to 9
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[0]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[0]->Character Index: From -1 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[0]->Primary Weapon Index: From -1 to 11
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[1]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[1]->Character Index: From -1 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[22: Name="e5_fld_inf1"]->Starting Locations[1]->Primary Weapon Index: From 3 to 11
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[24: Name="e5_fld_inf2_z"]->Primary Weapon Index: From 15 to 9
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[32: Name="e6_fld_inf2_a"]->Legendary Difficulty Count: From 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[34: Name="e6_fld_inf2_c"]->Legendary Difficulty Count: From 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[36]->Parent Squad Group: From 12 to 15
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[38: Name="e6_fld_inf5"]->Legendary Difficulty Count: From 6 to 12
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[63: Name="e12_pro_inf3_end"]->Major Upgrade: From Normal to Many
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[66]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[67]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[68]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[69]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[70]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[71]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Scripting Data[0]->Point Sets[1: Name='pelican1']->Points[1: Name='p3']->Position x: From 554.0562 to 549.0562
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[56]->Parent Squad Group: From -1 to 29
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6320]->Value: From (int16) 2 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6324]->Value: From (int16) 3 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6346]->Value: From (int16) 1 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6357]->Value: From (int16) 1 to 150 [-106,0]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6367]->Value: From (int16) 1 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6378]->Value: From (int16) 1 to 150 [-106,0]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6388]->Value: From (int16) 1 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6399]->Value: From (int16) 1 to 150 [-106,0]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6425]->Value: From (int16) 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6439]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6449]->Value: From (int16) 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6463]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6473]->Value: From (int16) 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6487]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6497]->Value: From (int16) 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6511]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6521]->Value: From (int32) 600 [88,2] to 1800 [8,7]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6528]->Opcode: From 18 to 16
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6533]->Value: From (int16) 3 to 0
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6585]->Opcode: From 18 to 16
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6590]->Value: From (int16) 3 to 0
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6639]->Value: From (int16) 3 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6660]->Value: From (int16) 90 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6661]->Value: From (int16) 150 [-106,0] to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6678]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6688]->Value: From (int16) 3 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6709]->Value: From (int16) 90 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6710]->Value: From (int16) 150 [-106,0] to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[6727]->Value: From (int16) 1 to 300 [44,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7156]->Value: From (int16) 0 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7183]->Value: From (int16) 0 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7200]->Value: From (int16) 0 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7478]->Value: From (int16) 2 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7482]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7507]->Value: From (int32) 40 to 41
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7508]->Value: From (int16) 2 to 4
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7511]->Value: From (int32) 40 to 41
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7512]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7536]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7580]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7624]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7652]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7690]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7727]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7764]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[7785]->Value: From (int16) 3 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8167]->Value: From (int16) 2 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8180]->Value: From (int16) 2 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8193]->Value: From (int16) 2 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8206]->Value: From (int16) 2 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8219]->Value: From (int16) 2 to 6
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[40]->Force Combat Status: From None to Alert
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8658]->Value: From (int16) 2 to 3
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8662]->Value: From (int16) 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8670]->Value: From (float) 0.2 [-51,-52,76,62] to 0.4 [-51,-52,-52,62]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[8672]->Value: From (int32) 600 [88,2,0,0] to 1800 [8,7,0,0]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9155]->Value: From (int16) 0 to 8
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9181]->Value: From (int16) 0 to 8
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9211]->Value: From (int16) 1 to 2
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9219]->Value: From (int16) 0 to 1
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9240]->Value: From (int16) 0 to 1
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9277]->Value: From (int32) 300 [44,1] to 900 [-124,3]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9414]->Value: From (int16) 2 to 12
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[9955]->Value: From (float) 3 [0,0,64,64] to 4 [0,0,-128,64]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[10785]->Value: From (int16) 150 [-106,0] to 450 [-62,1]
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Script Expressions[10894]->Value: From (int16) 1 to 3

[INCOMPLETE] Have Flood initially focus on other enemies by default during santified fight
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[54: Name="e10_pro_inf1_a"]->Legendary Difficulty Count: From 3 to 5
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[58: Name="e10_fld_storm"]->Flags->Follow Squad: From unchecked to checked
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[58: Name="e10_fld_storm"]->Follow Squad Index: From -1 to 54
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[58: Name="e10_fld_storm"]->Follow Radius: From 0 to 5

[INCOMPLETE] Add Grunts with Fuel Rod Gun to final fight
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[61: Name="e12_pro_inf2_left"]->Starting Locations[*]->Character Index: From * to 9
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[61: Name="e12_pro_inf2_left"]->Starting Locations[*]->Primary Weapon Index: From * to 14
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[62: Name="e12_pro_inf2_right"]->Starting Locations[*]->Character Index: From * to 9
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[62: Name="e12_pro_inf2_right"]->Starting Locations[*]->Primary Weapon Index: From * to 14

[INCOMPLETE] Disabled Active Camo on Flood Combat Forms
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[53: Name="e8_fld_inf1_z"]->Flags->Active Camo: From checked to unchecked
-Changed scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Orders[59: Name="e10_fld_storm_z"]->Flags->Active Camo: From checked to unchecked

[INCOMPLETE] Limit jackal snipers and flood snipers on High Charity to non-dark areas (and have flood snipers shoot longer range only on this level)
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[28: Name="e6_pro_inf3_a"]->Starting Location[3]->Character Index: From 15 to 14
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[28: Name="e6_pro_inf3_a"]->Starting Location[3]->Primary Weapon Index: From 12 to 2
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[29: Name="e6_fld_inf1"]->Starting Location[3]->Primary Weapon Index: From 11 to 1
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[54: Name="e10_pro_inf1_a"]->Starting Location[3]->Character Index: From 15 to 14
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[54: Name="e10_pro_inf1_a"]->Starting Location[3]->Primary Weapon Index: From 12 to 2
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[55: Name="e10_fld_inf1"]->Starting Locations[6]->Primary Weapon Index: From 11 to 6
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[55: Name="e10_fld_inf1"]->Starting Locations[*]->Placement Script: From * to <blanks>
-Change scenerios\solo\07b_forerunnership\07b_forerunnership.scnr->Squads[55: Name="e10_fld_inf1"]->Starting Locations[*]->Placement Script Index: From * to -1
-Change objects\characters\floodcombat_elite\ai\floodcombat_elite.char->Perception Properties[*]->Max Vision Distance: From * to 90
-Change generic.char->Weapons Properties[26: Weapon="sniper_rifle"]->Weapon Properties[26]->Maximum Firing Range: From 35 to 90

THE GREAT JOURNEY:

[INCOMPLETE] Made Brutes on Ghosts carry Brute Plasma Rifles (instead of regular Plasma Rifles)
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[3: Name="e1_pro_ghosts0_0"]->Primary Weapon Index: From 0 to 7
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[4: Name="e1_pro_ghosts0_1"]->Primary Weapon Index: From 0 to 7
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[5: Name="e1_pro_ghosts0_2"]->Primary Weapon Index: From 0 to 7

[INCOMPLETE] Have first Phantom not stay around so long
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[20321]: From (int32) 24 to (int32) 22

[INCOMPLETE] Have enemies driving wraiths be certain ranks
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[8: Name="e1_pro_wraith0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[15: Name="e2_pro_wraith0_0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[16: Name="e2_pro_wraith0_1"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[60: Name="e8_pro_wraiths0_0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[61: Name="e8_pro_wraiths0_1"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[62: Name="e8_pro_wraiths0_2"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[73: Name="e11_pro_wraith0_0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[74: Name="e11_pro_wraith0_1"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[75: Name="e11_pro_wraith1_0"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[76: Name="e11_pro_wraith1_1"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[77: Name="e11_pro_wraith1_2"]->Major Upgrade: From * to All
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[78: Name="e11_pro_wraith1_3"]->Major Upgrade: From * to All

[INCOMPLETE] Have allies follow you across the bridge
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[18911]: From (int32) 1 to (int32) 0
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[18962]: From (int32) 1 to (int32) 0
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Orders[70: Name="e5_cov_inf0_continue"]->Primary Area Set[0]: From Goal/7/11 to Goal/8/0
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Orders[70: Name="e5_cov_inf0_continue"]->Primary Area Set[1]: From Default/7/7 to Default/7/11

[INCOMPLETE] Have second Phantom show up earlier
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[18759]: From (int32) 36 to 27

[INCOMPLETE] Adjust enemy spawns throughout the level
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[3: Name="e1_pro_ghosts0_0"]->Normal Difficulty Count: From 4 to 5
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[3: Name="e1_pro_ghosts0_0"]->Legendary Difficulty Count: From 4 to 5
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[3: Name="e1_pro_ghosts0_0"]->Starting Locations[4]->Vehicle Index: From -1 to 3
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[20549]: From (int16) 1 to 2
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[20554]: From (int16) 3 to 4
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[20241]: From (int16) 10 to 11
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[19953]: From (float) 2 [0,0,0,64] to 4 [0,0,-128,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[19166]: From (float) 6 [0,0,-64,64] to 5 [0,0,-96,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[19169]: From (int32) 27 to 30
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[18715]: From (int32) 7 to 8
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Orders[79: Name="e5_pro_inf2_init"]->Order Endings->Triggers[0]->Trigger Index: From 42 to 43
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[47: Name="e6_pro_inf0_0"]->Legendary Difficulty Count: From 5 to 7
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[49: Name="e6_pro_inf0_2"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[49: Name="e6_pro_inf0_2"]->Legendary Difficulty Count: From 4 to 6
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[63: Name="e9_pro_inf0"]->Normal Difficulty Count: From 5 to 4
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[63: Name="e9_pro_inf0"]->Legendary Difficulty Count: From 5 to 4
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[63: Name="e9_pro_inf0"]->Major Upgrade: From Normal to None
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[63: Name="e9_pro_inf0"]->Starting Positions[0,1,3,4]->Flags->Always Place: From unchecked to checked
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[104: Name="boss_brute_start"]->Major Upgrade: From Normal to All

[INCOMPLETE] Added encounter where Phantom attacks scarab that you must fight off and removed 2nd spectre
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Scripts[423: e8_cov_inf0_main]: Changed to have index/salt of e9_pro_phantom0_main(393)
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[14536]: From (int32) 450 [-62,1,0,0] to (int32) 1800 [8,7,0,0]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[69: Name="e9_pro_spectres0_1"]->Normal Difficulty Count: From 2 to 0
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[69: Name="e9_pro_spectres0_1"]->Legendary Difficulty Count: From 2 to 0

[INCOMPLETE] Only have one banshee spawn at a time in the first wave during the scarab fight
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[14608]: From (int16) 1 to (int16) 0

[INCOMPLETE] Only two last banshees when scarab fires at door and last wraiths are destroyed
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[13388]: From (int16) 2 to (int16) 0
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[13432]: From (int16) 10 to (int16) 2

[INCOMPLETE] Have phantom deliver last wraith without waiting for scarab to open door or other wraiths to be destroyed
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[13354]: From (int32) 33 to (int32) 32
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[13348]: From (int16) 0 to (int16) 2

[INCOMPLETE] Have Johnson not crouch when firing at Tartarus and fire more often
-Changed [The Great Journey only] objects\characters\marine\ai\marine.char->Movement Properties->Flags->Disallow Crouch: From unchecked to checked
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1798]->From (float) 7 [0,0,-32,64] to (float) 6 [0,0,-64,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1802]->From (float) 15 [0,0,112,65] to (float) 8 [0,0,0,65]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1811]->From (float) 5 [0,0,-96,64] to (float) 6 [0,0,-64,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1815]->From (float) 12 [0,0,64,65] to (float) 8 [0,0,0,65]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1823]->From (float) 4 [0,0,-128,64] to (float) 6 [0,0,-64,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1827]->From (float) 10 [0,0,32,65] to (float) 8 [0,0,0,65]

[INCOMPLETE] Increased time for Tartarus' shield to recharge
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1741]->From (float) 1 [0,0,-128,63] to (float) 3 [0,0,64,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1745]->From (float) 2 [0,0,0,64] to (float) 3 [0,0,64,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1754]->From (float) 1 [0,0,-128,63] to (float) 4 [0,0,-128,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1758]->From (float) 3 [0,0,64,64] to (float) 4 [0,0,-128,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1766]->From (float) 2 [0,0,0,64] to (float) 5 [0,0,-96,64]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1770]->From (float) 3 [0,0,64,64] to (float) 5 [0,0,-96,64]

[INCOMPLETE] Have elite reinformements carry plama rifles and needler instead of needlers
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Squads[109: Name="boss_elite_reenforcements",111: Name="boss_elite_reenforcements_many]: Replace 5 (weapon index/secondary weapon index) with 0

[INCOMPLETE] Have reinforcements on regular intervals
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1859]->From (float) 60 [0,0,112,66] to (float) 20 [0,0,-96,65]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1872]->From (float) 60 [0,0,112,66] to (float) 20 [0,0,-96,65]
-Changed scenerios\solo\08b_deltacontrol\08b_deltacontrol.scnr->Script Expressions[1884]->From (float) 60 [0,0,112,66] to (float) 20 [0,0,-96,65]
