---
title: "Moon, the Game"
excerpt: "This is top down shoot-em-up game. <br/><img src='/images/MoonThumbnail.png' width='500' height='300'>"
collection: portfolio
---
{% include youtube.html id="hMQ7u0fNaBI" %}
You can find the [game and its demo here](https://github.com/bbernardoni/Moon/releases/tag/v1.0).

## About the project
This is a top down shoot-em-up game I created with a couple of friends. The player controls a woman in a prison facility on the moon who is trying to escape. They collect weapons and make their way out of the facility, either avoiding or fighting prison guards patrolling the area. 

## My Contributions
 <ul>
    <li>Wrote the game design documents for the project</li>
    <li>Implemented an A* pathfinding system developed by a 3rd party developer</li>
    <li>Developed AI for the actors in the maps so they can move around the map</li>
    <li>Developed a patrolling and alert system for NPC actors that included patroling along specified routes, aggressive behaviour, and searching</li>
    <ul>
        <li>Implemented different music for each state of alertness for NPCs on screen</li>
    </ul>
    <li>Developed character controls such as the following</li>
    <ul>
        <li>Movement around the map by walking and short burst dashing</li>
        <li>Aiming and firing weapons</li>
        <li>Switching weapons</li>
        <li>Interacting with objects</li>
    </ul>
    <li>Created pixel art for the main character</li>
    <li>Created and implemented animations for the main character</li>
</ul>

## Intentions & Process
This was the first project I finished on where I made a game design document. I teamed up with three others (two of whom worked with me on [VR Spaceship Dogfighting Simulator](https://arasyazgan.github.io/portfolio/portfolio-3/)) to bring this to life. We had originally intended to tell a story about a prisoner who was experimented on escaping a prison on the moon, including a dialogue system where NPCs would talk amongst themselves with text bubbles hanging overhead, and had intended to have several levels and different kinds of gameplay. However, we learned one of the most important thing: recognizing the limitations of budget and time, and planning your scope accordingly and realistically.

We wanted to make a game that encouraged players to take risks while being difficult. The core mechanice that allowed us to realize this goal was the dash, which gave the player significant mobility, while also allowing them to deal damage if they risked getting close to the enemy, and most importantly was the only source of healing (as the player could heal a significant amount of health by killing an enemy by dashing through them). This also allowed us to control the pace of the boss fights quite significantly. A potential boss we did not have time to implement would have had two phases, where they retreat after taking a certain amount of damage, and the player would instead have to face several weaker enemies that they could heal off of, allowing us to give the player a helping hand using the mechanics we had already established.

Another important mechanic was the enemy patrols and their aggressiveness system. The enemies in the prison would not automatically know where the player is, so they would patrol until the player came into sight, at which point the music would change and they would leave their original patrol route to attack the player. This allowed the player to approach the game as a stealthy escapee instead of a raging warrior who picks every fight they can.