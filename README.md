

## Duration

- 200 to 300ms for most animations.
- Hover transitions should be faster as our eyes are already focused on element.
- Heavy/big animations should be slower.

## Spring animations

- Are interruptable.
- Bounce is good for gesture based interactions.

## Easing

- **ease-out** for most scenarios. Great for user-intitated interactions as it has a snappy start.
- **ease-in-out** for items already on the screen that need to move to a new position. 
- **ease** is similar to ease-in-out but assymetrical -- faster start. Nice for hovers.

Custom curves for a bit more oomph.

:root {
  --ease-in-quad: cubic-bezier(.55, .085, .68, .53);
  --ease-in-cubic: cubic-bezier(.550, .055, .675, .19);
  --ease-in-quart: cubic-bezier(.895, .03, .685, .22);
  --ease-in-quint: cubic-bezier(.755, .05, .855, .06);
  --ease-in-expo: cubic-bezier(.95, .05, .795, .035);
  --ease-in-circ: cubic-bezier(.6, .04, .98, .335);
 
  --ease-out-quad: cubic-bezier(.25, .46, .45, .94);
  --ease-out-cubic: cubic-bezier(.215, .61, .355, 1);
  --ease-out-quart: cubic-bezier(.165, .84, .44, 1);
  --ease-out-quint: cubic-bezier(.23, 1, .32, 1);
  --ease-out-expo: cubic-bezier(.19, 1, .22, 1);
  --ease-out-circ: cubic-bezier(.075, .82, .165, 1);
 
  --ease-in-out-quad: cubic-bezier(.455, .03, .515, .955);
  --ease-in-out-cubic: cubic-bezier(.645, .045, .355, 1);
  --ease-in-out-quart: cubic-bezier(.77, 0, .175, 1);
  --ease-in-out-quint: cubic-bezier(.86, 0, .07, 1);
  --ease-in-out-expo: cubic-bezier(1, 0, 0, 1);
  --ease-in-out-circ: cubic-bezier(.785, .135, .15, .86);
}