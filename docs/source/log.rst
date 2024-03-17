Log
===
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
  
