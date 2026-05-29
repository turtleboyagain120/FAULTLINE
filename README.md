# FAULTLINE

FAULTLINE is a controller-first 2D parkour shooter built with HTML5 Canvas, CSS, vanilla JavaScript, Web Audio, and the browser Gamepad API.

Run across an endless brutalist rooftop skyline with elevated trains in the distance, chain movement tricks, fight red enemies, survive orange pressure units, collect drops, and push the run as far as you can.

## Contact

For questions, feedback, bugs, or ideas:

**timmytheonlinegirl@hotmail.com**

## How To Play

Open `index.html` through a local server, then press **START RUN** from the main menu.

FAULTLINE is designed for controller play first. Keyboard and mouse still exist as fallback/testing input, but the intended layout is controller-only.

## Goal

- Move fast.
- Stay alive.
- Kill enemies.
- Collect ammo, hearts, shields, coins, weapons, rescue gear, and power cubes.
- Use checkpoints.
- Survive boss prompts.
- Keep pushing through the endless generated rooftop route.

Falling does not instantly restart the whole game. It costs health and returns you to a checkpoint when one is available.

## Controller Controls

| Input | Action |
|---|---|
| Left stick | Run, move in menus, and air-turn while airborne |
| Right stick | Aim weapon and rotate the body while airborne |
| A | Jump, double jump, vault from cover, select menu item |
| LT | Slide / crouch |
| LT tap then A | Air strafe boost |
| RT | Fire equipped weapon |
| RT with no ammo | Assisted melee |
| LB | Dash burst |
| RB | Shotgun burst |
| X | Assisted combat mode |
| B | Cycle weapon to the right |
| Y | Reload |
| Start | Pause / resume menu |
| D-pad | Move through menus |
| D-pad right | Try to grab a rare ragdoll guard |

## Movement

FAULTLINE is built around momentum. You accelerate, slide, jump, double jump, wall jump, dash, air-turn, and vault from cover. The player does not stop instantly, so good movement feels like chaining tricks instead of pressing one button at a time.

## Slide And Air Strafe

Air strafe is the big movement combo:

- Tap LT.
- Release it.
- Press A quickly.
- If the timing is right, you get a fast air-strafe boost.
- Air-strafe lasts around 3.8 seconds.
- Holding LT while air-strafing gives extra precision only during that active air-strafe.

Crouching in normal air does not give the precision boost.

## Combat

The main weapon is an AR. Other weapons can drop during the run.

- AR: steady default weapon
- SMG: fast spray weapon
- Pistol: slower backup weapon
- Shotgun: close-range emergency burst

Player bullets have light tracking, but they do not fully aim for you. Weak spots can stagger enemies and reward ammo or shield value.

## Melee

If every gun is empty, RT becomes assisted melee so you are not helpless. Melee can mix punches, kicks, and elbows. X can also start assisted combat manually.

## Health And Shields

The player has:

- 5 hearts
- 2 shield armor slots

Enemy bullets are dangerous. Shields absorb damage first. Shield drops have a chance to restore 1.5 shield armor.

## Enemies

Enemies can patrol, shoot, dodge, jump, strafe, rush, guard, suppress, and attack close range. The level generator spaces enemies so they should not spawn stacked on top of each other.

Enemy types include:

- Regular red enemies
- Orange elite pressure units
- Turrets
- Bonus bosses
- Evil twin / boss encounters

## Orange Enemies

Orange enemies are rare and scary. They can have shields, shoot often, strafe into the air, and trigger a takedown prompt. If the prompt appears, follow the shown stick or button instruction quickly.

## Bosses And Tactic AI

Bosses use prompts and can copy habits you overuse. For example, if you keep air-strafing, a boss may trigger **BOSS COPY** and briefly move like it learned your air tactic.

Tactic AI is not internet AI and it does not call an outside service. It is a local in-game director that watches recent player actions, stores simple memory, predicts likely tactics, and lets enemies or bosses choose better responses.

## Random Level Machine

Each run uses a fresh seed. The level machine streams sections in front of the player and cleans old content behind the camera. It builds from validated pieces, checks spacing, avoids recent repeats, and mixes polished rooftop themes like roof decks, skyways, cranes, and radio towers.

## Rooftop Visual Theme

The whole game now uses a polished rooftop identity with distant city motion in the background.

- The background uses layered city buildings, clouds, rain, neon windows, and skyline fog.
- Drones, cable cars, and distant elevated trains move through the background so the skyline still feels alive.
- Running platforms use rooftop props like vents, water tanks, cranes, skyway rails, and radio equipment.
- The basement trap still has its own 430-frame fight loop near the bottom entrance.

## Power Cubes

Hit a glowing power cube to trigger overdrive. Overdrive temporarily grows the player, increases reach, makes weapons feel bigger, and helps during difficult fights.

## Pickups And Inventory

Enemies can drop ammo, shields, hearts, coins, weapons, and rescue gear. Auto Inventory can help with weapon choice, reload timing, pickup priority, reserve ammo behavior, and weapon swapping.

## Menu Settings

### Smoothing

Adds a motion-smoothing visual effect. Turn it off if the game feels blurry or slower.

### Tactic AI

Enables extra enemy prediction settings:

- Memory
- Prediction speed
- Influence
- Focus
- Debug view

### Auto Inventory

Helps with weapon and ammo decisions:

- Weapon preference
- Reload behavior
- Pickup behavior
- Ammo reserve behavior
- Swap behavior

### Stick Response

Changes controller stick behavior:

- Expo: smoother and more precise near the center
- Linear: direct stick response

Expo is the default.

### Movement Assist

Keeps movement beginner-friendly. Hardcore makes movement less forgiving.

### Comfort FX

Reduces intense visual effects like shake and rain.

### Reticle Size

Switches between normal and large reticle.

## Major Update, ELI5

The big update made FAULTLINE easier to understand and more alive.

- The start menu now shows a real gamepad diagram instead of plain text boxes.
- The instructions now match the current controller-only layout.
- The game now uses a polished rooftop theme with skyline layers, distant elevated trains, rooftop props, drones, cable cars, cranes, and radio towers.
- Bosses now have a visible **BOSS COPY** moment when they copy your repeated tactic.
- The AI menu wording is cleaner: it is now called Tactic AI because it controls enemy prediction and decisions.
- Tips explain the actual current game: endless rooftops, shields, air strafe, boss prompts, weak spots, pickups, and troubleshooting.

ELI5 version: the game now tells you what to press, the world is a rooftop city with moving background traffic, bosses show when they learn from you, and the basement has a long looping background fight.

## Troubleshooting

### The controller does not work

Connect the controller, press a button, then reload the page if needed.

### The game feels blurry

Turn off Smoothing from the menu.

### Movement feels too twitchy

Use Stick Response Expo and keep Movement Assist on.

### The game is visually too intense

Turn Comfort FX on.

### I am out of ammo

Use RT for assisted melee, or cycle weapons with B to check another weapon.

### I fell

Falling costs health and returns you to a checkpoint when available.

### I am stuck

Open the pause menu with Start and choose New Run.

## Files

Main browser game files:

- `index.html`
- `styles.css`
- `game.js`
- `assets/685206__x1shi__video-game-music-seamless.wav`
- `assets/476818__victorium183__menuaccept.wav`

## License

FAULTLINE is released under the Apache License 2.0.

Copyright 2026 turtleboyagain120.

See `LICENSE` for the full license text.
