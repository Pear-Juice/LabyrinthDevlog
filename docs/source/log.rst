Log
===
Thursday: 4/4/24
  | "Swapped" animated sprite for animation player and animation tree which took forever
  | Result is a cleaner code that is somewhat more powerful and can do things like trigger sound effects in sync with animation
  | Consequence being my sanity
  | Next thing to do is move away from animation and movement code and make save points an actual game mechanic though if I am feeling bored I can either work on spring ability or some more animating

Wednesday: 4/3/24
  | Thoughts on the gameplay loop: Robots require power and recharge stations must be found. Recharge stations can also work as spawn points
  | Rooms when they move should visibly shift this could be done on rails? Moving rooms while you are in the could create extremely interesting gameplay

Tuesday: 4/2/24
  | Drew so so many animations
  | Jumping, jump release, running jump and release, slink run, beginnings of wall slide and climb, etc
  | Overall cat is looking much more complete 

Wednesday: 3/20/24
  | Most creatures that are fast should have limited range
  | Break tone armor by having most enemies unable to follow between rooms
  | Creature ideas:
  | Snake like things hiss hiss
  | Many legs grab
  | Things that go pop

Tuesday: 3/19/24
  | Notably being written at 4 am after having listened to too many Magnus Archives episodes. Inspiration afoot.. Thoughts on moving towards a more horror esc vibe as I cannot think of a single horror skill platformer and I can only imagine. Also been thinking about redesigning the character for many days now and I'm thinking something with claws.. I can imagine some cool animations surrounding sliding down walls and leaving scratch marks. Recently I watched a video from Jonas Tyroller about optimal searching for game direction and how at the beginning many new ideas should be tested as well as large direction jumps can be incredibly necessary. This to me feels like I landed on something gold. Plus I've kinda wanted to make something horror for a while now.
| 
| Possible idea for game beginning: Walking up to a massive wall, camera zooming in as you approach. Enter a pillared corridor with graffiti on the wall saying something like ye who enter, perish yada yada, stay out. Then big sliding door and fade to black.
|
| Idea for character weapon and smash ability. They carry a chain hook which  grapples and pulls towards walls. A dagger to slash with. And combining the two to reel in enemies into the dagger for massive damage. Later have upgrades for barbed hook and such.
|
| Multiple phases for hook: Pull, pull a d slide, pull and bounce
| 
| Possession of enemy ability? Current control system could make this extremely feasible as enemies could use the same input tags as the player. Difficulty comes from reassigning things like camera to the enemy and allowing it through door transitions but that should be simple. Possession should last until the enemy dies in which the player resumes from where it was before possession. This could work as a way to explore inaccessible areas or function similarly to Celeste binoculars. Best way to write this in will be to further decouple what a player is which should give the ability to reassign the player to any other suitable creature. Possible methods for balancing include time limits, damage on exit as if the host takes notice and licks you out, and possibly visual restrictions depending on the creature.

Monday: 3/18/24
  | Fixed bugs surrounding coyote time and jump queuing. Half was leftover from debugging wall jump + smash with a cheeky return statement at the beginning of the input function. Non goofy mistakes were having time checks for input time stamp and ground / wall hit timestamp flipped. I do not know how I only realized now.
  |
  | Built a fun testing area for smash bounces capability. Turns out it's a lot and a Celeste recharge system might be needed for balancing and control over uses

Saturday: 3/16/24
  | Moving faster than default movement speed into left wall smash would not bounce, velocity calculations were at fault and is now fixed

Thursday: 3/15/24
  | Made faster velocities than default movement speed persist even after touching the ground
  | This came as a result of modifying the movement code to make anything that moves you faster than default movement speed not have the requirement of holding the desired direction immediately or holding no button at all
  |
  | This when changed was decided to be a feature but it is notably very broken and allows for infinite accumulation of velocity. Making levels that can't easily be cheesed may be a problem 
Wednesday: 3/14/24 (And earlier dates)
  | Wow it has been a minute since I've updated this
  | Fixed so many bugs with smash bounce
  | Fixed wall jump to smash not bouncing
  | Added wall smash bounce modifier
  | Made smashing preserve velocity
  | Tweaked bounce pad's launce force
  | Solidified art style to be drawn flat color and stylistic and mostly monochrome
  | Added in two new areas designed to teach smash bounce ability
  | Placed half blocks everywhere to make wall jump training a little easier, still need to play test with those who are not familiar with wall jumping
  | Playtested playtested playtested, who knew it is so hard to teach people how to use a complex ability. Can't wait to teach diagonal smash woohoo
  | Figured out that the very first challenge everyone gets stuck on in the same way, swapping around the first and last challenges of that room should fix it
  | Fixed player able to trigger other room switchers whilst switching by teleporting them far away during. This does cause a 1 frame flicker meaning some transition might be needed
  | That's all folks, hope to keep logs a little more consistent

Thursday: 2/29/24
  | Finished smash bounce code, animation is pending till art style has been solidified
  | Created three new areas at the beginning of the game for skill training
  | Changed naming system from coordinates to description of purpose
    | This means areas can be put between  other areas without the need to rename every single other room. It also works to better identify what each room is and create purpose for why it exists 
    | This does make conceptualizing space more difficult and will make an external program necessary to keep track necessary in the future 

Tuesday: 2/27/24
  | Bugfixing smash bounce ability
  | Created three new rooms

Wednesday: 2/21/24
  Fixed walljump height so you cant climb walls infinitly

Tuesday: 2/20/24
  Begun drawing backgrounds
  Questioning current visual style as there is no vibe
    | Background and foreground should not be separate
    | Foreground is too flat even though there is plenty of color depth
    | How important is vibe? Many games don't have a vibe but still have a cohesive style
  Tested out parallax layers and an example background and found parallax layers do not inherit parent visibility 

Monday: 2/19/24
  Fixed portals spawning you far away from area boundaries
    Simply realized that exit area2d was not used and that shifted everything inward
  
