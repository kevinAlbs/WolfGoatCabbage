Finishing basic state transitions
- Going to bed, animals leaving
- Picking up gun, standing by lake
- Make a function like:

function onBoundChange(left, right, insideAction, leftAction, rightAction) {}
Use for boat, barn, lake, etc. or maybe onEnterLeft, etc...

Clean up code
- Consider push vs pull. Right now polling is inefficient but nicer to code, can pushing also be
done nicely?
- States like x coordinate make sense to pull since each movement would have to notify all listeners.

Extras:
- Write WebGL filter for zoom blur or something.
- Auto shadows