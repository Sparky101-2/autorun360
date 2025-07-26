# autorun360 - a Titan 2 script that provides a 360° autorun feature for fixed-view games like Diablo IV

## What is it

Ever wished autorun worked properly in games with locked camera angles? This [Titan 2](https://www.consoletuner.com/products/titan-two/) script makes that happen. It gives you 360° autorun in games like [Diablo IV](https://diablo4.blizzard.com) — where direction isn’t camera-relative, but fixed.

Most autorun scripts default to holding the stick forward, which doesn't work in games with a fixed camera. This one adjusts input direction dynamically — so if you’re moving right on-screen, the stick is pushed right accordingly.

Using autorun360 feels intuitive:

- Whilst autorun360 is on, you can change the direction by moving the left stick in any direction near to the outer  edge (i.e. with a stick strength > 85).

- Autorun360 will continue in the direction that you last pointed the Left stick in.

## Trigger customisation

The way I have implemented the triggers for enabling and disabling the autorun360 function is:

>**TO START** - R-stick   UP > 85 strength   **AND**   L-stick >85 strength (in any direction)
>
>**TO STOP**  - R-stick DOWN > 85 strength

This just happens to fit my Diablo 4 Necromancer build which doesn't rely on the right stick for targeting enemies.

However, you can fairly easily change the triggers to whatever you want.

For example you could choose to use L3 to toggle enabling/disabling the function.

## BONUS: Useful generic functions

This project has some functions which can be reused and may be useful in other scripts:

`int getStickAngle360(fix32 x, fix32 y)`

- takes the (x,y) coords of the controller stick position, and outputs the angle. ONLY returns 0-359 (and not 360)

and

`uint8 getStickStrength(int stick_angle, fix32 x, fix32 y)`

- returns an integer in the range of zero to 100 indicating how far the stick is from the centre (0) to the outer edge (100)

## List of other games with locked camera angles
The following is a list of games with fixed camera angles that may also benefit from using this script.

- Path of Exile (PoE, PoE2)
- Torchlight III
- Pillars of Eternity II: Deadfire
- Pathfinder: Wrath of the Righteous
- Alienation
- Victor Vran
- Baldur’s Gate III
- Little Nightmares
- Limbo
- Inside
- Tormented Souls
- Gauntlet: Slayer Edition​
- Bastion
- The Ascent
- Pillars of the Earth
- Disco Elysium – The Final Cut

## Final thoughts

While working on this, I was also developing edge-scanner — the two projects evolved side by side, and [edge-scanner](https://github.com/Sparky101-2/edge-scanner) turned out to be an indispensable part of making this one possible.

Appreciate you checking this out — if it helped, [please drop a thanks here](https://www.reddit.com/r/TitanTwo/comments/1m8u5o8/360_autorun_is_finally_here_t2_script_for_diablo/)!

## Keywords (for search matching)

titan-two, Titan 2, Titan2, Titan Two, TitanTwo, gpc, gtuner, script, console, psn, ps4, ps5, ps6, playstation, xbox

auto run, autorun, 360, peripheral, periphery, outer edge, outer limit, scan, calibration, calibrated, calibrate
