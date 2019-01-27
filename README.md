# BrickRigs-physics-patch
Unofficial fix for the bouncing bug on the roads in the racetrack, city and desert maps in Brick Rigs.

## Installing
Copy the UserEngine.ini file to [BrickRigs.exe folder]/BrickRigs/Config/ (create this folder if it doesn't exist).

## Notes
I am in no way affiliated with the creator of Brick Rigs and this is an unofficial modification for the game. But somebody told me the developer of this game claims that this simple fix I proposed will impact performance too much. In my opinion this is probably the most ignorant and pathetic way of saying that you don't care at all about your game. After all, Brick Rigs is a CAR building game. And you CAN'T EVEN DRIVE ON ROADS AT REASONABLE SPEEDS. I left the Brick Rigs community after I heard that.

## Performance Impact
This patch is currently configured in a way that will eliminate almost every possible physics glitch when driving on roads. This also means that it will have a performance impact on CPU-bound systems.

On the testing machine with a low-end 2009 AMD Phenom II X2 550 this can lead to an fps drop of up to ~10-15% when 2000+ bricks are in the scene. However, by increasing the maximum allowed delta time for a single iteration you can lower the performance cost in exchange for less fidelity in the physics simulation.
