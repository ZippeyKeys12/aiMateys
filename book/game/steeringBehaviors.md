# Steering Behaviors

Steering behaviors use a collection of forces in order to produce realistic movement.
While the individual elements may be simple, their combination can cause the emergence of complex behavior.

They function on an ideal direction and subtracting the actor's velocity from it to get a steering force:

`steering=normalize(idealVelocity-velocity)*maxSteer`

## Seek

The *seek* behavior's ideal direction is the vector from the actor to their target:

`idealVelocity=normalize(targetPosition-position)*maxVelocity`

## Flee

The *flee* behavior's ideal direction is the opposite of the *seek* behavior's:

`idealVelocity=normalize(position-targetPosition)*maxVelocity`

## Pursue

The *pursue* behavior seeks the next place the target will be. This is done by adding the target's current velocity to it position.

`idealVelocity=normalize(targetPosition+targetVelocity-position)*maxVelocity`

## Evade

The *evade* behavior uses the same logic as the *pursue* behavior as an addition to the *flee* behavior as opposed to *seek*.

`idealVelocity=normalize(position-(targetPosition+targetVelocity))*maxVelocity`