# CRT

A TouchDesigner component that draws the input as a signal on a CRT tube. The shader runs on a GLSL TOP. Controls live on the parent CRT page.

Output resolution is the GLSL TOP's own resolution. Scanlines follow the input line count. The phosphor mask follows output pixels.

## Parameters

- **Geometry** — tube curvature, zoom, corner radius, vignette.
- **Scanlines** — beam depth and width, line count (0 uses the input height), signal gamma.
- **Mask** — mask type (none, aperture, slot, shadow), strength, triad pitch in pixels, brightness boost.
- **Glow** — halation of bright areas, radius, threshold, and diffusion through the glass.
- **Signal** — chromatic aberration, noise, flicker. Time comes from `absTime.seconds`.
- **Grade** — brightness, contrast, saturation, bezel darkening.
