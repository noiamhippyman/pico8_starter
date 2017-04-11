# Hippyman's Pico-8 Starter Project
This is a good generic starting point for any Pico-8 game project.

Usage:
Open Pico-8 and type "folder" and press enter
Drag "starter.p8" and "starter_example.p8" into your projects folder
Type "load starter" into Pico-8 and press enter
Type "save 'gamename'" where 'gamename' is whatever you want
You can now begin working on your game


API:
game:new_actor(x,y) - Creates a new actor instance. Returns ActorID
game:update() - Updates any existing actor instance animations
game:render() - Renders any existing actors instances to the screen
game.background_color - Sets the color of the screens background

new_anim(start,length) - Creates an animation to store in actor anims table

index_from_2d(x,y,row) - Finds index in 1D array from 2D coordinates. row is the width of the 2D area
x_from_index(index,row) - Finds x position from index. row is the width of 2D area
y_from_index(index,row) - Finds y position from index. row is the width of 2D area

insert(list,pos,value) - inserts a value into a table and shifts values where necessary

actor.x,actor.y - Actor position
actor.img - Actors current sprite
actor.imgspd - Speed of animation
actor.depth - Handles what is in front and what is behind actor. Lower values are drawn last
actor.flipx,actor.flipy - Booleans that handle which way sprite is flipped
actor.anim - index of current animation
actor.anims - table that holds all actor animations
actor:update() - Called automatically in game:update. This updates the animations
actor:draw() - Called automatically in game:render. This renders the actor to the screen
