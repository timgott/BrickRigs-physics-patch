# BrickRigs-physics-patch
Unofficial fix for the bouncing bug on the roads in the racetrack, city and desert maps in Brick Rigs.

## Notes
I am in no way affiliated with the creator of Brick Rigs and this is an unofficial modification for the game. Still I would be very happy to see this change in the game, especially considering how simple it is.

## Performance Impact
This patch is currently configured in a way that will eliminate almost every possible physics glitch when driving on roads. This also means that it will have a performance impact on CPU-bound systems.

On the testing machine with a low-end 2009 AMD Phenom II X2 550 this can lead to an fps drop of up to ~10-15% when 2000+ bricks are in the scene. However, by increasing the maximum allowed delta time for a single iteration you can lower the performance cost in exchange for less fidelity in the physics simulation.

## Installing
Copy the UserEngine.ini file to [BrickRigs.exe folder]/BrickRigs/Config/ (create this folder if it doesn't exist).

That's it!
