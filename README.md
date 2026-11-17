# Gorilla-Gore
||THIS MOD WAS MADE WITH CLAUDE. WHICH MEANS THAT THIS IS VIBECODED||

IN THE GAME
-----------
B (right controller)  open / close the menu. Press its buttons with a fingertip.
  Color            R, G and B sliders, 0 to 9 like the game's color picker. Slide your finger along them.
  Name             a keyboard. Up to 12 letters and numbers. DEL removes the last one, Done goes back.
  Spawn            a gorilla in that color, with that name over its head, in front of you.
  Weapons          pick a weapon for your right hand (press it again, or Put Away, to put it away).
  Clear Gorillas   removes all of them and the blood.
Punch                 swing an empty hand into a gorilla fast. Harder punches knock it further, draw blood,
                      and enough of them knock a part off.
Grip                  grab a gorilla (or any piece of one). Let go while moving your hand to throw it.
Grip with both hands  on two parts of one gorilla, then pull your hands apart to rip it.

WEAPONS (right hand; while you hold one, that hand does not grab or punch)
  Knife     slash across a gorilla to cut it open; thrust the point in to stab (it pumps blood).
  Axe       chop hard: it knocks the gorilla away, breaks bone and takes limbs off in one or two blows.
  Pistol    trigger fires. Headshots count far more; a few burst the head.
  Shotgun   trigger fires 9 pellets, then it pumps itself.
  Grenade   hold the trigger to pull the pin (the fuse is burning!), let go of the trigger to throw.
  C4        trigger throws a charge that sticks to whatever it hits (a gorilla too). A sets them all off.
  Explosions burst gorillas close by, tear limbs off further away, and set off other bombs nearby.

Only works offline or in MODDED lobbies. In a normal lobby the menu closes and the gorillas go away.


config.cfg  (the numbers)
----------
Open it with Notepad. Changes are picked up while the game is running (within 2 seconds).
  [Spawn]  Red / Green / Blue / Name   what the menu set (Red/Green/Blue = -1 copies your own color)
           ShowName, NameHeight         the name tag above the gorilla
           Distance, MaxGorillas        where they appear and how many at once
  [Gore]   BloodAmount (0 = no blood), ImpactDamage, Toughness, RipDistance
  [Punch]  MinSpeed (how fast a punch must be), Strength
  [Weapons] Damage, ExplosionSize, GrenadeFuse; HoldPitch / HoldForward if weapons sit wrong in your hand
  [Grab]   ThrowBoost, GrabRadius
  [Sound]  Volume (0 to 1)
Delete config.cfg to get all the default values back.


textures\  (the pictures)
---------
Replace a picture with your own of the SAME NAME (.png, or .jpg if you don't need see-through parts).
Restart the game to see the change. Delete a file to get the original back.
Files you have not changed are replaced automatically when the mod is updated; yours are never touched.
  spatter1.png, spatter2.png, spatter3.png   blood splats left on the floor and walls
  drops.png                                  small blood drops
  spray.png                                  puffs of blood spray in the air
  flesh.png                                  the meat inside wounds, torn ends and gibs
  knife_0, axe_0, pistol_0, shotgun_0, grenade_0, c4_0 (.jpg)   the weapons' colours (knife_2 and knife_4 too)
  the weapons' .png files with odd numbers (pistol_1 ...)        their normal maps (surface bumps), not colours
Pictures with transparency should be PNG. Square sizes like 256x256 or 512x512 work best.


sounds\  (the sounds)
-------
Replace a sound with your own .wav of the SAME NAME (MP3/OGG must be converted to WAV first,
e.g. with Audacity: File > Export > WAV). Any sample rate, mono or stereo.
Restart the game to hear the change. Delete a file to get the original back.
Files you have not changed are replaced automatically when the mod is updated; yours are never touched.
Sounds with numbers are "takes" of the same thing; one is picked at random each time. You can ADD
more takes by continuing the numbers (e.g. gush10.wav, gush11.wav ...).
  bone1-12      bones breaking           crunch1-4     bone crunches     snap1-3    sharp cracks
  rip1-5        flesh ripping            riplong       a long rip (torso torn in half)
  tear1-10      wet tearing              stab1-5       stabs             pop        a part bursting
  gush1-9       blood gushing out        drip1-10      single drips      driploop   steady dripping
  splat         blood landing            squish1-6     squishes (grabbing, pieces landing)
  punch1-6      punches landing          flesh1-6      fleshy impacts    slap1-5    wet slaps
  thud1-5       body hitting the ground
  scream1-7     the gorilla screaming (big injuries)     grunt1-14   pain grunts (knocks and punches)
  pistol1-3     pistol shots             shotgun1-3    shotgun blasts    pump1-3    shotgun pump
  explosion1-3  explosions               bullethit1-8  bullets in flesh  ricochet1-2  bullets off walls
  swing1-3      blade swishes            shell1-3      cases landing     pin1-2     grenade pin     beep   C4 beep
To silence one sound, replace it with a very short silent .wav.
