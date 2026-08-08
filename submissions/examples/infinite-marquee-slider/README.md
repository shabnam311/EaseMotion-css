# Infinite Marquee Slider Component

A pure CSS implementation of a seamless, infinitely scrolling marquee. This pattern is heavily used on modern marketing sites to display "Trusted By" logo carousels or looping text banners.

## Features
- **Zero JavaScript**: Powered entirely by CSS `@keyframes` and `transform: translateX`. No complex JS math to calculate element widths or clone nodes on the fly.
- **Seamless Looping**: By duplicating the inner `.marquee-group` exactly once, and shifting the track by `calc(-100% - var(--marquee-gap))`, we achieve a flawless, infinite visual loop.
- **Pause on Hover**: The `animation-play-state: paused` rule allows users to stop the scrolling by hovering over the track, improving UX and readability.
- **Accessible**: Fully respects `@media (prefers-reduced-motion: reduce)`. If enabled, the animation is permanently paused and the wrapper becomes horizontally scrollable `overflow-x: auto` instead, ensuring content remains accessible without inducing motion sickness.

## Usage
Open `demo.html` in your browser. The mock company names will slowly scroll from right to left.
- Hover your mouse over any block to pause the entire track.
- The gradient fades on the left and right edges are implemented as absolute overlays that match the background color, creating a smooth entrance and exit effect.

## Files
- `demo.html`: The HTML structure demonstrating the original group and the duplicate group (which receives `aria-hidden="true"` to prevent screen readers from reading the content twice).
- `style.css`: The styling rules containing the keyframe logic and layout handling.
