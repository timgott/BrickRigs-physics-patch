# BrickRigs-physics-patch
Unofficial fix for the bouncing bug on the roads in the racetrack, city and desert maps in Brick Rigs.

## Installing
Copy the UserEngine.ini file to [BrickRigs.exe folder]/BrickRigs/Config/ (create this folder if it doesn't exist).

## How it works
BrickRigs simulates aerodynamics, collisions and suspensions, which means the engine has to solve high-order nonlinearities. If the time step is too large, the integration approximation will stray too far from the exact solution, resulting in glitches. Usually this can be done a lot better with a high fixed update rate. By default, BrickRigs is configured to run at a variable physics step synced with rendering, which turns out to be too imprecise for simulation of vehicles at higher speeds. 

The config file simply increases the possible update rate to solve these issues. This also means that it will have a performance impact on CPU-bound systems, although it should be noted that BrickRigs is a vehicle building game and without this patch you can't take a single lap on a racetrack without your vehicle randomly exploding.

Additionally you will notice that suspensions behave a lot more nuanced than before, especially when turning.

## Performance Impact
This patch is currently configured in a way that will eliminate almost every possible physics glitch when driving on roads. 
On the testing machine with a low-end 2009 processor this can lead to an fps drop of up to ~10-15% when 2000+ bricks are in the scene. 

However, by increasing the maximum allowed delta time for a single iteration you can lower the performance cost in exchange for less fidelity in the physics simulation.

## Notes
I am in no way affiliated with the creator of Brick Rigs and this is an unofficial modification for the game.
