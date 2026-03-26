Description
-

Flattened is a mod for Human: Fall Flat.

The download link was originally on MediaFire, but GitHub is much better since there are no annoying pop-ups or anything. Plus I can add the older versions of the mod, although they may no longer be compatible with the game.

Special thanks to Durf for creating the Hooman mod which got me into making this, and the creator of this post/website:
https://human.rlybtd.com/1287.html?btwaf=95520805
It told me how to skip the into credits with some code.

Guide
-
This guide can also be found in the Info.txt file.

### Keybinds:
Gravity:
- Numpad:
  - (1) - 1/1 Gravity
  - (2) - 1/2 Gravity
  - (3) - 1/3 Gravity
  - (0) - 0 Gravity
  - (Plus) - Increase gravity by 0.1
  - (Minus) - Decrease gravity by 0.1
  - (Left Shift) - Increase speed of gravity increases and decreases
- Number Key Row:
  - (1 + Right Shift) - 1/1 Gravity
  - (2 + Right Shift) - 1/2 Gravity
  - (3 + Right Shift) - 1/3 Gravity
  - (0 + Right Shift) - 0 Gravity
  - (Plus + Right Shift) - Increase gravity by 0.1
  - (Minus + Right Shift) - Decrease gravity by 0.1
  - (Left Shift) - Increase speed of gravity increases and decreases


### Commands:

#### Targets:

Some commands have a (target) parameter. This is what that means.

| Target | Description |
| --- | --- |
| (player) | Player number identified from using "/list" command in chat |
| others | All players except the host of the server |
| all | All players |
- - -
#### chaos
Format:
| Command | Description |
| --- | --- |
| chaos | Toggles chaos mode |

Every 20-60 seconds, chaos can either:
1. Suddenly change the gravity, sometimes to an extreme degree
2. Suddenly give players extreme super strength, which makes picking up objects far too easy as they go flying upwards, resulting in the player losing grip
3. Suddenly give players extreme weakness, which does the opposite of super strength
4. Enter "Jumpy time" which decreases gravity, then increases it, then repeats 20-40 times
- - -
#### gravity
Format:
| Command | Description |
| --- | --- |
| gravity | Displays the current gravity values |
| gravity (x) (y) (z) | Sets gravity forces on XYZ plane to the XYZ values given ("0, -9.81, 0" is default) |
- - -
#### pos
Format:
| Command | Description |
| --- | --- |
| pos (player) | Displays targeted player's coordinates |
- - -
#### savepos
Format:
| Command | Description |
| --- | --- |
| savepos (name) (player) | Stores the position of the targeted player, and saves it under the assigned name |
| savepos (name) (X) (Y) (Z) | Stores the position of the XYZ coordinates, and saves it under the assigned name |
| savepos list | Displays all saved positions |
| savepos (name) remove | Removes the position with the assigned name |
| savepos clear | Clears all saved positions |
- - -
#### tp
Format:

  "tp"
    Tip: Teleporting to yourself may help if stuck somewhere
    Format:
      tp (target) (player)               -   Teleports target to player
      tp (target) (X) (Y) (Z)            -   Teleports target to XYZ coordinates
      tp (target) (name)                 -   Teleports target to saved position

  "ungrab"
    Format:
      ungrab (target) (time)             -   Disables grabbing for target for specified time

  "ragdoll"
    Format:
      ragdoll (target) (time)            -   Makes target unconscious for specified time

  "mass"
    Format:
      mass (player)                      -   Displays mass of player
      mass (target) (mass)               -   Sets mass of target

  "weight"
    Format:
      weight (player)                    -   Displays weight of player
      weight (target) (weight)           -   Sets weight of target

  "liftforce"
    Format:
      liftforce (player)                 -   Displays liftforce of player
      liftforce (target) (liftforce)     -   Sets liftforce of target

  "pushforce"
    Format:
      pushforce (player)                 -   Displays pushforce of player
      pushforce (target) (pushforce)     -   Sets pushforce of target

  "reset"
    Format:
      reset (target)                     -   Sets mass, weight, liftforce, climbforce, and pushforce of target back to default values

  "waterbreathe"
    Format:
      waterbreathe (target) (true/false) -   Sets waterbreathing for target to true or false

  "fly"
    Format:
      fly (target) (true/false)          -   Sets flying for target to true or false

    To fly, press the jump button in the air, then extend either one or two arms, and press or move a movement button/stick. You fly in the direction you are looking.
    Use one hand for the minimum flying speed, and use both hands for the maximum flying speed.
    Hold the "play dead" or unconscious button to not grab things while flying.
    To stop flying, press the jump button in the air again.

  "flyspeed"
    Format:
      flyspeed (player) (min/max)           -   Displays either minimum or maximum flying speed of the player
      flyspeed (target) (min/max) (speed)   -   Sets either minimum or maximum flying speed of the target to the specified speed
      Recommended Speeds:
        Min: 20
        Max: 50

  "collide"
    Format:
      collide (target) (true/false)      -   Sets collisions of target to either true or false

  "superpunch"
    Format:
      superpunch (target) (true/false)   -   Enables or disables super punch ability of target

    To punch, extend an arm and press the "play dead" button at the same time.
    All of the human body, except its arms, will freeze. As long as either arm is still extended, the body will remain frozen.

  "punchstrength"
    Format:
      punchstrength (player)             -   Displays punch strength of player
      punchstrength (target) (strength)  -   Sets punch strength of target to given value
      Recommended Strength:
        100,000 or above

  "superspeed"
    Format:
      superspeed (target) (true/false)   -   Enables or disables super speed ability of target

    To start running, hold the "play dead" button while walking. You can turn the camera to change direction, or move using the directional buttons while keeping the camera still.

  "speed"
    Format:
      speed (player)                     -   Displays super speed value of player
      speed (target) (strength)          -   Sets super speed value of target to given value
      Recommended Speed:
        30 to 60

  "flashtime"
    Format:
      flashtime (no parameters)          -   Displays the current flashtime value
      flashtime (0.01 <= value <= 1)     -   Sets flashtime value to a number from 0.01 to 1

    To enable flashtime, press the "play dead" button and the jump button at the same time. You must have superspeed to be able to do this.

  "exitflashtime"
    Format:
      exitflashtime                      -   Exits flashtime

    This is useful in case someone in flashtime leaves, or loses superspeed. If that happens, no player will be able to exit using the buttons. This command solves that problem.

  "speedtrail"
    Format:
      speedtrail (target) (true/false)   -   Enables or disables speed trails for superspeed, trail will also appear during wall running if superspeed is enabled

  "trailcolor"
    Format:
      trailcolor (player)                -   Displays speed trail color of player
      trailcolor (target) (color)        -   Sets the speed trail color of target

  "wallrun"
    Format:
      wallrun (target) (true/false)      -   Enables or disables wall running for target

    To wall run, move towards a wall and hold jump. If you stop moving, you will stay stuck to the wall until you let go of jump, or move away from the wall.

  "flips"
    Format:
      flips (target) (true/false)        -   Enables or disables flips for target

    To flip, press jump while in the air.
    You can do different flips depending on which direction you are moving
    Double jump: Don't move
    Front flip: Move forwards
    Left flip: Move left
    Right flip: Move right
    Backflip: Move backwards

  "sprint"
    Format:
      sprint (target) (true/false)        -   Enables or disables sprinting for target

    To toggle sprint, press ragdoll. Your sprint speed depends on your run speed value.

  "webs"
    Format:
      webs (player)                      -   Displays whether player has webs enabled, and if true, it displays the web mode
      webs (target) (simple/manual)      -   Sets web mode of target to either simple or manual
      webs (target) false                -   Disables webs for target, it only disables, because the way for enabling webs is "simple" or "manual" instead of "true"

    Manual Webs:
    Extend either arm, press and tap ragdoll to shoot web
    The webs will stay in your hands until you release them
    To release the webs, extend the hand you want to release webs from (it can be both hands), and tap jump
    This way, you can hold on to one web, but let go of the other, obviously. Just wanted to point out the manual quality.
    If one hand is holding multiple webs, and you extend that hand and press jump, all webs from that hand will be released.
    The main reason for the ability to hold multiple webs in one hand is purely because Spider-Man 2 :)

    Simple Webs:
    Press and hold ragdoll, web stays attached while ragdoll is held
    The hand that shoots the web is random if not grabbing anything
    If left hand is grabbing, only right hand shoots a web
    If right hand is grabbing, only right hand shoots a web
    The web doesn't attach to anything, it's positioned above the player and slightly forwards in the direction the player is facing.

  "webstrength"
    Format:
      webstrength (player)               -   Displays web strength of player
      webstrength (target) (strength)    -   Sets the web strength of target

  "webcolor"
    Format:
      webcolor (player)                -   Displays web color of player
      webcolor (target) (color)        -   Sets the web color of target

  "heatvision"
    Format:
      heatvision (target) (true/false)   -   Enables or disables heatvision for target

    To use heat vision, hold ragdoll. The lasers will shoot in the direction you look.
    If your lasers hit an object that is affected by physics, it will push it back an amount depending on the laser force of the player.
    If your lasers hit a player, they will respawn, unless they are invincible.

  "laserforce"
    Format:
      laserforce (player)                -   Displays heat vision laser force of player
      laserforce (target) (value)        -   Sets heat vision laser force of target to value

  "lasercolor"
    Format:
      lasercolor (player)                -   Displays heat vision laser color of player
      lasercolor (target) (color)        -   Sets the heat vision laser color of target

  "combat"
    Format:
      combat (target) (true/false)   -   Enables or disables combat for target

    A player has a health value, an energy value, and a strength value
    If the energy value drops to 0, the player is knocked out for 1.5 seconds
    If the health value drops to 0, the player respawns with full health and energy
    The greater the player's strength, the more knockback the attacks produce
    If the player that is hit is invincible, no damage is dealt

    Left punch: Hold ragdoll and extend left hand
    Right punch: Hold ragdoll and extend right hand
    Kick: Hold ragdoll and press jump

  "health"
    Format:
      health (player)                -   Displays health of player
      health (target) (value)        -   Sets health of target to value

  "energy"
    Format:
      energy (player)                -   Displays energy of player
      energy (target) (value)        -   Sets energy of target to value

  "strength"
    Format:
      strength (player)                -   Displays strength of player
      strength (target) (value)        -   Sets strength of target to value

  "invincible"
    Format:
      invincible (target) (true/false)        -   Enables or disables invincibility for target

  "superjump"
    Format:
      superjump (target) (true/false)   -   Enables or disables super jump for target

    To super jump, hold jump to charge your jump, then release jump to jump
    The total charge time is 3 seconds
    The greater the jump strength, the higher the jump, although values that are too high result in glitching

  "jumpstrength"
    Format:
      jumpstrength (player)                -   Displays jump strength of player
      jumpstrength (target) (value)        -   Sets jump strength of target to value

  "showfpsbody"
    Format:
      showfpsbody        -   Enables or disables player visibility for first-person camera

  "buildmode"
    Format:
      buildmode (target) (true/false)        -   Enables or disables build mode for target

    Extend right hand and hold ragdoll to create path of cubes
    Grab with right hand to delete grabbed object
    Careful when deleting level objects! It can cause severe glitches. Deleting players is not recommended. Deleting the cubes you've placed should be fine however.

    Extend left hand and press ragdoll to create one cube
    Grab with left hand to rotate grabbed object

    The cube size is set with "buildsize" command
    The cube distance is set with "builddist" command
    The cube color is set with "buildcolor" command

  "buildsize"
    Format:
      buildsize (player)                -   Displays build size of player
      buildsize (target) (value)        -   Sets build size of target to value

  "builddist"
    Format:
      builddist (player)                -   Displays build distance of player
      builddist (target) (value)        -   Sets build distance of target to value

  "buildcolor"
    Format:
      buildcolor (player)                -   Displays build color of player
      buildcolor (target) (color)        -   Sets build color of target to color

  "skip"
    skip                                 -   Skips the intro credit animations. Running this after the credits have passed will cause an error in the console.
