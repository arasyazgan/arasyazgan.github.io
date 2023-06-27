---
title: "Mechmania 25 and 26"
excerpt: "Mechmania is a yearly hackathon where competitors create an AI that can play a specific game against the bots created by other players. I was one of the developers creating the yearly games. <br/><img src='/images/MM25Thumbnail.png' width='480' height='360'>"
collection: portfolio
---
{% include youtube.html id="YQr96-xllmU" %}

## About the project
I was part of the Mechmania development team for two years while I was a student at the University of Illinois (UIUC). These games were made by teams of volunteers during school years. All members participate in the initial game design and prototyping process, where we would try and iterate on various ideas on physical mediums. Once we finalized our game design documents, each year, the Mechmania (MM) team would split into 5 teams: game design, art & graphics, visualizer, engine, and infrastructure. 

## My Contributions
During MM 25, I was a part of the visualizer team (5 out of the 30 people working on the project). Each team controlled three characters in the form of mechs on a grid map with obstacles and various environmental hazards. On each turn in a 3-turn round, each team moved a single character up to its movement, and made attacks in custom player made patterns. These moves were done simultaneously between both teams. After a certain point, the map would start shrinking by dropping bolders on the outermost ring of tiles. Whichever team survived while the opposing team had no remaining characters alive won the match.
<ul>
    <li>Implemented animations, models, and visual effects for all moving parts of the game</li>
    <li>Designed the placement and implemented the animations of the UI elements</li>
    <li>Provided live site support and debugging during the competition, when unexpected errors and bugs appeared</li>
    <li>Detected errors in the game engine's code and its erroneous communication of the coordinates of map elements</li>
</ul> 

The next year, during MM26, I played a more prominent role in the visualizer team, as we were only a team of two. A lot of the Mechmania team's veteran members had to leave, and so this was a more turbulant development cycle, however we were able to complete the game in time as planned. This game had all of the players in a large map, and several private maps, where they compete for resources, equipments, and points. I did the following: 
<ul>
    <li>Developed code to translate the package of the game state sent by the game engine team into movements of the actors on the visual board</li>
    <li>Implemented and fixed visuals for character equipment by closely working with the art team</li>
    <li>Provided live site support and debugging during the competition, when unexpected errors and bugs appeared</li>
</ul> 

## Intentions & Process
Two very important considerations in the Mechmania games are that (a) the players are not human, but bots programmed in a matter of hours during this 24-hour competition, and (b) it must be entertaining to watch, potentially more so than it is to be "played". Consideration (b) is especially vital in the visualizer department, which is where most of my contributions lie.

For Mechmania 25, this was a straightforward challenge, if not an easy one. At any given time, only two players were on the field. We decided to focus on the living player pieces and moved the camera accordingly. To make a battle of supposedly giant mechs on a board come to life as a turn based game, I drew inspiration from various games that used VFX to create exciting and cool looking abilities in other such turn-based strategy games, such as Final Fantasy Tactics and Into the Breach. I found models for boulders, and VFX for smoke and fire. Since the game was being played by computers, it was relatively fast paced. Using the smoke trails and the fire, I created animations of rockets flying out of the screen and falling down from the atmosphere. Similarly, I set a pattern to the falling of the boulders when the arena shrinks so that it would feel more dynamic.