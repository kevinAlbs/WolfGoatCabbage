Features not in the game
------------------------
- Have the goat run away from wolf during the end sequence
- Combine the foreground images
- Write WebGL filter for ending effects
- Automatically generate shadows: flip, scale, rotate, erode, recolor
- Redo the stair animation and movement
- Add a periodic goat noise with sound distance

Browser Bugs
------------
IE 11
- Sound isn't multiplexed

Edge
- Keys for isDown stick very badly

Firefox
- When developer tools are opened, the sound is paused but never unpaused.
This might be partly firefox specific, but it's unclear. Was able to workaround by using audio tag:
```
PhaserGlobal = {
    disableWebAudio: true
};
```

And disabling mute on pause:
```
game.sound.muteOnPause = false;
```

However, doing so led to the issue that if you lose focus from the page, the audio will not loop
properly, and instead run into the next marker!

Audio seems to be a bit of a deeper issue. Namely, even using one sound object with allowMultiple
set to true doesn't seem to work in chrome.

Safari
Audio won't play on the first load of the page, see issue here: http://www.html5gamedevs.com/topic/19761-safari-and-problem-with-sound/?_fromLogin=1
The fix proposed didn't work for me, I was able to work around with manually calling game.sound.update() and context.resume() if it was detected, but I'd like to take a deeper look.
