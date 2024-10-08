---
title: "VR Spaceship Dogfighting Simulator"
excerpt: "This is spaceship and mecha VR game I developed in Unity. <br/><img src='/images/SpaceFlightVRThumbnail.png' width='500' height='300'>"
collection: portfolio
---
{% include youtube.html id="qsU2yLjkGsI" %}
You can find the [game and its demo here](https://github.com/Sketching101/moon2/releases/tag/v1.1).

## About the project
This is a VR game I created with a couple of friends. It is a game where the player controls a spaceship that can also transform into a mech (akin to a Gundam) powered with rocket launched fists, swords that slice ships and asteroids in two, and guns. The gameplay focuses on flight and space combat against other spaceships.

## My Contributions
- Created and filled the design documents for the game
- Developed all player controls, such as:
    - The ship's pitch, yaw, and roll controls
    - The ship's acceleration
    - The ship's transformation to and from mecha form
    - The ship's smart aiming and lock-on mechanics
    - The mecha's rocket punch and its maneuverability
    - The mecha's hands' ability to grip weapons, enemy ships, and asteroids
    - The mecha's ability to fire from guns and finger guns
    - The mecha's weapons fading in when being used, and fading out when not being used
- Created borders and UI elements to prevent the ship from getting lost in the vastness of space

## Intentions & Process
This project started as a simple VR flight game as part of our VR game development class at UIUC. I found this as the perfect opportunity to make a game that would excite me to play. Most of my design decisions throughout this process were based around this philosophy of "what's exciting?" While many people might assume a flight game could be difficult to play due to the nausea VR might cause when there's large amounts of movement, I found that as long as there was a motionless framework around you (such as the cockpit of an airplane) this common problem could be circumvented. I developed the framework for the flight mechanics and shooting while preparing this simple flight simulator. The controllers had no direct control over the ship by themselves. Instead, there were two objects in the cockpit: a joystick and a throttle. The throttle moved around 120 degrees, and how forward it was determined the ship's acceleration and decceleration (to a limit). The joystick's rotation affected the ship's pitch, yaw, and roll. The player could hold these objects and move them by moving their controllers, and depending on what they were holding, the buttons on the controllers would have different effects, such as firing lasers or lock on rockets, and moving the smart-targetting reticle.

After I built this skeleton, I teamed up with a couple of friends (the same people I worked with on [Moon, the Game](https://arasyazgan.github.io/portfolio/portfolio-4/)) to bring this airplane to the stars. The first and most important step was to add a second throttle which would change our spaceship into a spacefaring mech, akin to those seen in GUNDAM, Gurren Lagann, and Pacific Rim. When you pull on this throttle overhead, your ship's wings rotate to become your legs, and arms manifest slowly through the use of shaders, along with holographic weapons in your cabin. I considered what the mech form could do for the player, as it leaves them immobile. I decided to add finger guns (guns you can fire by making finger guns holding your controller, and fire by tapping your thumb on the controller's analog stick) because that felt like a silly thing. The next thing I added was perhaps a bit more silly, and definitely significantly more fun: rocket arms. The mech could now launch and direct its rocket propelled fists through space, knocking away enemy ships and asteroids.

The final key items were the weapons that manifested in the mech's hands when the player grabbed their holographic counterparts within the cockpit (two swords and two pistols). I found a package on the Unity Asset Store where someone had implemented code that could cut meshes along a plane during runtime. I implemented this package so that if the sword cut through something, that mesh would be split in two. A few seconds after the object was split in two, in order to add an "anime-like" effect where we often see something react to being cut moments after it has been cut, a force would be applied in opposite directions on the two objects so they would rapidly drift apart. While this was originally difficult to use due to the lack of mobility while in mech form, the rocket punch capability of the mech could be used while holding weapons, which meant the mech could send its deadly sword flying forward to asteroids and ships alike. The gun on the other hand could be fired as if firing a gun with the handle identical to the controller.

The player could easily shift between the ship form and the mech form. My teammates worked on AI that could work as adversaries for the player to test their mettle and arsenals against. I implemented two different maps for this game, but ran into an unforeseen issue in space, that was not present on earth: there is very little to anchor yourself around. I opted to create a cage around these two regions so that the players could see the borders of the world and not be surprised when a warning message shows up on their screen. This worked surprisingly well, but had the large downside of damaging the players' immersion. With more time, I intended to add more static structures and make the border in such a way that you would only see it if you reached a certain proximity to it.