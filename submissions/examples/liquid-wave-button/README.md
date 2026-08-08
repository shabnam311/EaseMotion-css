# Liquid Wave Button Component

A mesmerizing, pure CSS interactive button that simulates a liquid filling effect when hovered. This component uses clever `border-radius` manipulation and infinite rotation to create organic, wave-like shapes.

## Features
- **Zero JavaScript**: Entirely powered by CSS pseudo-elements (`::before`, `::after`), `@keyframes`, and `transform`.
- **Organic Fluid Dynamics**: By rotating slightly irregular border radii (`45%` and `40%`) at different speeds overlapping each other, it creates the illusion of splashing liquid.
- **Accessible**: Fully respects `@media (prefers-reduced-motion: reduce)`. For users with motion sensitivity, the infinite rotation is disabled. Instead of a churning wave, the button provides a clean, solid block color fill on hover, removing any nausea-inducing movement while preserving the interaction cue.

## Usage
Open `demo.html` in your browser. 
Hover over the buttons to see the liquid level rise up and fill the button background while the text color smoothly inverts.

## Files
- `demo.html`: The HTML structure containing the base button and the inner `.liquid` container element.
- `style.css`: The styling rules where the magic of the `animate-wave` rotation and absolute positioning lives.
