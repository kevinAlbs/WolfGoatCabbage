Bugs
----
- Gun pickup location
- You can ride back on the boat during a restart menu
- Farmer can walk beyond first boundary!
- Farmer walks during transitions...
- Red flash no longer works
- Farmer does seem to move out of bed if he goes outside before sleeping oddly enough

Code cleaning
-------------
- Change strings to const's
- Add consts for all magic numbers
- Consider using Phaser camera bounds for camera follow logic

Artwork
-------
- Add homelike items to barn
- Add z-indexes layers
- Water movement please!!!
- Remove shadows during night transition

Misc
----
- Add sound effect for gunshot
- Add idle animations for wolf and goat, move around sometimes

Extra
-----
- Have goat run away from wolf during end sequence
- Consider best speed for ending music fade-in
- Write WebGL filter for zoom blur or something.
- Auto shadows
    + Flip, scale, rotate, ERODE!
- Decision trees for state transition logic
- Make mute button in Phaser, not HTML (scaling better, more consistency)