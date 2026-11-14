# Skyshift — SPHEREx Time Explorer

Skyshift is a beginner-friendly public-facing prototype for the NASA Space Apps 2026 SPHEREx challenge. It lets a visitor move between NASA-published SPHEREx observations of interstellar comet 3I/ATLAS from August and December 2025.

## Open the project

Open `index.html` in a modern web browser. An internet connection is needed to load NASA's hosted image files and source pages.

## What works

- Timeline slider switches between the two observation campaigns.
- Play button automatically moves between the campaigns.
- Each selected image has its own date, caption, and official NASA source link.
- Explanations describe what a comet's coma is and what the reported brightening means.
- The page clearly says these are separately processed NASA-published views, not a calibrated, pixel-aligned difference image.
- Links take visitors to NASA's image gallery, the IRSA 3I/ATLAS data page, and the SPHEREx Data Explorer.

## Data used

NASA's image gallery describes SPHEREx observations of 3I/ATLAS during August 7–15 and December 8–15, 2025. The page uses the NASA-hosted August campaign GIF and a NASA/JPL-Caltech December SPHEREx image. NASA's December photojournal article reports that the comet brightened significantly during that campaign. The app links to both primary source pages and the underlying calibrated images in IRSA.

The displayed campaign visuals are genuine NASA-published SPHEREx imagery, but they are not identical calibrated cutouts processed for direct pixel subtraction. The prototype therefore supports a visual, educational comparison and does not claim to detect or measure a change automatically. A science-grade follow-up would query the IRSA observation table, download compatible FITS images, align the sky coordinates, check pixel flags and uncertainties, and only then calculate a difference map.

## Attribution

Image credits: NASA/SPHEREx and NASA/JPL-Caltech. Archive and calibrated spectral image data: NASA/IPAC Infrared Science Archive (IRSA). This student prototype is not an official NASA product.

## Suggested improvements

1. Use the IRSA comet observation table to list individual observations and timestamps.
2. Let visitors filter observations by wavelength and date.
3. Process matched FITS cutouts into aligned images and add an uncertainty-aware difference view.
4. Add keyboard controls and screen-reader descriptions for the timeline.

The page styling lives in `styles.css`; keep it in the same folder as `index.html` when moving or sharing the project.
