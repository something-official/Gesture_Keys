# Gesture Keys

Gesture Keys explores the bridge between spatial input and ordinary web controls. Pointer hover and click work immediately; a future landmark provider can supply the same normalized coordinates.

## What this demonstrates

- Mapping normalized coordinates to a grid of key rectangles
- Separating hover feedback from activation
- Designing a pointer fallback before adding a landmark model
- Keeping generated text in an accessible live region

## Run it

Open `index.html` in a modern browser. For camera mode, serve the folder from localhost or HTTPS and choose **Start camera**. No npm, bundler, or build step is required.

## Browser and privacy notes

Camera permission is requested only after a user action, video-only constraints are used, frames are processed locally, and tracks stop on page exit. Pointer and sample modes remain available when permission is denied or tracking is unavailable. This is an educational visual lab, not a medical, security, or measurement-grade product.

## How to study this

Start with `index.html`, then inspect the `signalNow()`, `draw()`, and mode-specific renderer in `app.js`. Change one mapping at a time and keep the fallback understandable before adding a model or external dependency.

## License

Released under the MIT License. See [LICENSE](LICENSE).
