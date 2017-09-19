# canvas-browser-game
experiment creating a canvas browser game.

This is an experiment creating a canvas-based browser game. Preferably multiplayer.
I'm thinking a top-down adventure-type game.

So I'd like to create a circle and move it around.
I'd like that action to be cross-browser.

I'd like game state to be persisted somehow.
And reloadable.

Should I use a game engine?
I found this comparison: https://github.com/showcases/javascript-game-engines
It looks like Phaser is the most popular. Let's see what it offers:
Phaser 2.8.7 is the most recent.
http://phaser.io/download/stable
The api seems straightforward. It lets you do things like:
```
    player = game.add.sprite(32, game.world.height - 150, 'dude');
    // and
    game.physics.startSystem(Phaser.Physics.ARCADE);
```
Cool.
```
// Built-in keyboard manager.
cursors = game.input.keyboard.createCursorKeys();
```
Nice.

Get started says to npm install. Fair enough.
How to serve?
Just include the phaser repo on the frontend and load phaser on window.onload.

Fair enough.
Ok, what's next? Some ideas...
Adventure-game. Should it have multiple screens? How to generate the map? I need some art. opengameart is a good source.
Alternatively, I could use vector graphics. In some ways that's more interesting.
I have an idea for an auto-generated maze-like map where a man is stuck and trying to find the exit,
perhaps while being chased by someone else trying to catch him.

Sounds good to me.

I created a Sara character and a Bran character.
Bran:
http://gaurav.munjal.us/Universal-LPC-Spritesheet-Character-Generator/#?body=darkelf2&eyes=yellow&nose=big&ears=elven&legs=robe_skirt&clothes=longsleeve_brown&mail=none&armor=none&jacket=none&hair=long_raven&gloves=none&weapon=none&ammo=none&shield=none
Sara:
http://gaurav.munjal.us/Universal-LPC-Spritesheet-Character-Generator/#?sex=female&eyes=blue&nose=button&legs=sara&clothes=tunic_teal&mail=none&armor=none&hair=swoop_white_cyan&hairsara-toplayer=0&hairsara-bottomlayer=0&hairsara-shadow=0&arms=none&hat=none&hats=tiara_purple&gloves=golden&shoes=slippers_white&buckle=none&quiver=none&bracelet=none&cape=none&necklace=none

Sara and Bran would be in a forest.

I thought I would download Tiled to create a map.

I created a little map.

Next I would need to put the characters on the map.

