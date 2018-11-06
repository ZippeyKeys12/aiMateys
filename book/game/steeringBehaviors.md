# Steering Behaviors

Steering behaviors use a collection of forces in order to produce realistic movement.
While the individual elements may be simple, their combination can cause the emergence of complex behavior.

They function on an ideal direction and subtracting the actor's velocity from it to get a steering force:

```steering=normalize(idealVelocity-velocity)*maxSteer```
