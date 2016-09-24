Bugs
----

Code cleaning
-------------
- Change strings to const's
- Add consts for all magic numbers
- Consider using Phaser camera bounds for camera follow logic

Artwork
-------
- Add homelike items to barn
- Add z-indexes layers
- Remove shadows during night transition
- Fix night transition

Misc
----
- Add sound effect for gunshot, (goat?), footsteps?
- Add idle animations for wolf and goat, move around sometimes
- Ending music should be programmatic (noise should fade in as function of step)

Extra
-----
- Have goat run away from wolf during end sequence
- Consider best speed for ending music fade-in
- Write WebGL filter for zoom blur or something.
- Auto shadows
    + Flip, scale, rotate, ERODE!
- Decision trees for state transition logic
- Make mute button in Phaser, not HTML (scaling better, more consistency)