# Scan

Grayscale scanline effect. Brightness shifts the phase of a cosine carrier. The result is quantized, smoothed, and written back as brightness.

## Parameters

- **Rate** — carrier frequency.
- **Depth** — modulation depth.
- **Steps** — quantization steps.
- **Drift** — phase shift, in radians.
- **Smooth 1–3** — the first three smoothing filters.
- **Cutoff** — fourth filter. 0.05 or higher turns it off.
