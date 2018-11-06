# Steering Behaviors

Steering behaviors use a collection of forces in order to produce realistic movement.
While the individual elements may be simple, their combination can cause the emergence of complex behavior.

They function on an ideal direction and subtracting the actor's velocity from it to get a steering force:

```steering=normalize(idealVelocity-velocity)*maxSteer```

## Seek

The *seek* behavior's ideal direction is the vector from the actor to their target:

```idealVelocity=normalize(target-position)*maxVelocity```

## Flee

The *flee* behavior's ideal direction is the opposite of the *seek* behavior's:

```idealVelocity=normalize(position-target)*maxVelocity```

