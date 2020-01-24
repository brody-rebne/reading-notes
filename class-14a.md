# CSS Transformation

## Transform
- Different types with values in parens
- Common types:
  - rotate(60deg) - rotates object
  - `scale(1.3)` (+ scaleX/scaleY) - resizes object
  - `translate((25px)` (+ translateX/translateY)  - moves the object in a direction
  - `skew(7deg, 18deg)` - skews the object from multiple corners
- Multiple transform values can be applied
- To apply multiple transforms, list them both in the same property value
- The `transform-origin` property sets the position at which the transformation begins
- The `perspective` property sets the depth of the effect, effectively setting the vanishing point for the transform
- `perspective-origin` sets the offset of the perspective point's placement

## Transitions
- Can set multiple styles for objects based on states, using pseudoselectors
- Transitions are used to determined how the object transitions between styles
- Not all properties can be used with transitions
- Properties with identifiable halfway points can be transitioned
- `transition-properties` sets properties which will be affected by the transition
- `transition-duration` sets how long the transition will take (usually in s or ms)
- `transition-delay` is used to set a delay on the transition
- These properties can be declared in shorthand within the `transition` selector (similar to `border` or `box-shadow`)

## Animations

- Set with the `@keyframes` rule
- Use keyframes (progress points within the animation duration) to set more complex transformations
- Can set completely different states for the object's styling for each keyframe declared
- Keyframes use % values
- `animation-name` used to apply the animation to an element
- Various properties like duration, timing, and delay can be set with modifier properties on the element
- Can be iterated