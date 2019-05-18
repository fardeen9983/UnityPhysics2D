# 2D physics in Unity
All objects in 2D plane are limited to movement in XY plane with z axis component as zero. The physics componenets of 3D are present sd their 2D counterparts in the 2D physics engine. We can have both 2D and 3D objects in the same scene but they wont interact with each other. The overall physics settings for the game can be modified through the Physics 2D component in the Player settings.

To make a game engine fall under the command of 2D physics engine simply add a RigidBody2D component to the object. This also opens up physics control and adding joint components

Different colliders in 2D physics : Circle, edge, polygon and box colliders

## Rigid body 2D
It is a game component taht allows 2D objects to be affected by 2D physics. It also needs to be attached to a collider. It is used to define physical properties like mass, drag, affection to gravity and allowing ading 2D joints etc. Gravity can be set on a scale per object basis.

To interact physically all participating game objects need to have a rigid body 2D property. The collider will be automatically added and needs to be sized accordingly relative to objects size.

The fixed angle features allow physics interaction but not with angular rotation. Physics operation can be smoothed out through interpolation. It has a sleeping mode for none, awake and asleep. It will wake up and interact on collisions or before them.

Collision detection : dicrete is used mostly and concrete for fast moving objects.

## Collider 2D
To have a physical presence and have it's shape and presence defined objects need to have collider 2D component attached to them.

Different types of colliders
1. Circular
2. Box
3. Edge
4. Polygon

Polygon and edge colliders are pretty similar as they are formed by connecting edges but they differ in the fact that polygon collider represents closed shapes while the later, open edge connections.

All colliders share properties like physics material 2D which define bounciness and fricitions of collision and is trigger defines if colider will participate in collision  or let objects pass through. 

The collider can be adjusted so it's bounadary matches with the object itself using SHift key in the scene. This can also be used to create new edges and vertices in polygon and edge collider. To delete a vertex in such collider click on it while holding the ctrl key

Add colliders only and no rigid bodies to static objects
## Hinge joint 2D 
Such joint allow a 2D object to rotate about an axis while being fixed at a point. The point about which it rotates is defined by the Connected body Rigid body field which can be a fixed point in space or a game object with a rigid body.

Other properties include anchor and connected anchor points. 
* Anchor is the point around which the sprite rotates around
* Connected anchor defines where in the scen this point is placed and is relative to the connected item

Collide connected sets whether the object will collide with the connected body.

We can add motors to add velocity and rotation to the joint and apply limits to the min/max angle to which it can be rotated.