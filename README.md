# Collage Studio

A modern, browser-based collage editor for creating custom image layouts quickly and intuitively.

Collage Studio runs entirely in the browser and provides a collection of ready-made layouts, adjustable dividers, custom-drawn layouts, image positioning controls, and high-resolution PNG and JPG export — without requiring a backend or external framework.

## Features

* **Multiple collage layouts**

    * Single image
    * Rows and columns
    * Grid and masonry layouts
    * Diagonal layouts
    * Magazine-style layouts
    * Panorama and featured-image layouts
    * Circle-focus layout
    * Custom-drawn layouts

* **Custom layout editor**

    * Draw your own dividers directly on the canvas
    * Move existing dividers while preserving their angle
    * Delete individual divider segments
    * Detach connected segments
    * Undo custom layout changes
    * Snap new dividers to 15° increments with `Shift`

* **Adjustable dividers**

    * Drag layout handles to resize individual sections
    * Divider positions are stored separately for each layout
    * Double-click or double-tap a divider handle to reset it

* **Drag & drop image editing**

    * Drag images inside their slots
    * Drag images between collage slots
    * Reorder loaded images
    * Replace or remove individual images
    * Drop image files directly onto collage slots

* **Image zoom and positioning**

    * Zoom slider
    * Ctrl/⌘ + mouse wheel zoom
    * Pinch-to-zoom on touch devices
    * One-click image centering

* **Collage customization**

    * Adjustable gap size
    * Adjustable corner radius
    * Custom background color
    * Multiple aspect ratios:

        * 1:1
        * 4:5
        * 3:2
        * 16:9

* **High-resolution export**

    * PNG export
    * Optimized JPG export
    * Export preview
    * Multiple output widths:

        * 1200 px
        * 1600 px
        * 2048 px
        * 3000 px

* **Responsive design**

    * Desktop and mobile layouts
    * Touch-friendly controls
    * Mobile gestures
    * Safe-area support

* **Automatic dark mode**

    * Follows the operating system's preferred color scheme

* **Built-in localization**

    * English
    * Hungarian
    * Language is selected automatically from the browser settings

## Getting Started

Collage Studio is a client-side application and does not require a build process.

You can use the hosted version directly in your browser:

**[Open Collage Studio](https://lkristof.github.io/collage-studio/)**

Alternatively, clone the repository and serve it with any static web server.

## Usage

1. Choose a collage layout.
2. Select the desired aspect ratio.
3. Click **Images** to add photos, or drop them directly onto the collage.
4. Drag an image to reposition it inside its slot.
5. Use the zoom control, pinch gesture, or Ctrl/⌘ + scroll to resize the selected image.
6. Drag divider handles to customize the layout.
7. Adjust the gap, corner radius, and background color.
8. Choose an export resolution.
9. Click **Export** and save the collage as PNG or JPG.

### Swapping images

Press and hold an image, then drag it onto another collage slot to swap their positions.

### Custom Draw Mode

Select **Custom draw** to build your own layout.

With drawing enabled:

* Drag across the canvas to create a new divider.
* Hold `Shift` while drawing to snap the divider to 15° increments.
* Drag an existing divider to move it while keeping its angle.
* Click or tap a divider segment between intersections to delete or detach it.
* Use **Undo** to revert the latest custom layout change.

Custom layouts support up to **12 slots**.

## Project Structure

The application is intentionally lightweight.

```text
collage-studio/
├── index.html
├── site.webmanifest
└── assets/
    └── images/
        ├── apple-touch-icon.png
        ├── favicon.ico
        ├── favicon.svg
        ├── favicon-96x96.png
        ├── web-app-manifest-192x192.png
        └── web-app-manifest-512x512.png
```

The main application logic, styles, UI, layout definitions, image interactions, localization, and export functionality are implemented directly in `index.html`.

## Technology

Collage Studio is built with standard browser technologies:

* HTML5
* CSS3
* Vanilla JavaScript
* Canvas API
* Pointer Events
* File API
* Web App Manifest

No frontend framework or runtime dependency is required.

## Privacy

Images are processed locally in the browser.

The application does not require images to be uploaded to a server in order to create or export a collage.

This makes Collage Studio suitable for working with images locally without introducing a server-side image-processing pipeline.

## Browser Support

Collage Studio is designed for modern browsers with support for:

* HTML Canvas
* Pointer Events
* CSS `clip-path`
* CSS backdrop filters
* File and Blob APIs
* Modern JavaScript

For the best experience, use a current version of Chrome, Edge, Firefox, or Safari.

## Contributing

Contributions, bug reports, and feature suggestions are welcome.

If you would like to contribute:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Test them on both desktop and mobile.
5. Open a pull request.

## Icons

The user interface uses icons from [Lucide Icons](https://lucide.dev/), licensed under the ISC License.

## License

This project is available under the MIT License. See the [LICENSE](./LICENSE) file for more information.
