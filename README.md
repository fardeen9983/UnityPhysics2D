# 2D physics in Unity
All objects in 2D plane are limited to movement in XY plane with z axis component as zero. The physics componenets of 3D are present sd their 2D counterparts in the 2D physics engine. We can have both 2D and 3D objects in the same scene but they wont interact with each other. The overall physics settings for the game can be modified through the Physics 2D component in the Player settings.

To make a game engine fall under the command of 2D physics engine simply add a RigidBody2D component to the object. This also opens up physics control and adding joint components

Different colliders in 2D physics : Circle, edge, polygon and box colliders

## Rigid body 2D
It is a game component taht allows 2D objects to be affected by 2D physics. It also needs to be attached to a collider. It is used to define physical properties like mass, drag, affection to gravity and allowing ading 2D joints etc. Gravity can be set on a scale per object basis.

To interact physically all participating game objects need to have a rigid body 2D property. The collider will be automatically added and needs to be sized accordingly relative to objects size.

The fixed angle features allow physics interaction but not with angular rotation. Physics operation can be smoothed out through interpolation. It has a sleeping mode for none, awake and asleep. It will wake up and interact on collisions or before them.

Collision detection : dicrete is used mostly and concrete for fast moving objects.