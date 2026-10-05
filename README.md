# 3D Living Room

An interactive 3D living room built with plain HTML5, CSS3, JavaScript (ES6) and Bootstrap 5 (components and Bootstrap Icons). There is no framework, canvas or WebGL: the whole room is made of CSS 3D transforms.

## Run it

Open `index.html` in a modern browser. An internet connection is needed once to load Bootstrap, Bootstrap Icons and Google Fonts from CDNs.

## Features

- **CSS 3D room**: floor, three walls, sofa, coffee table, rug, bookcase, window, plant and floor lamp, all generated from a small `box()` / `plane()` helper in JavaScript.
- **Camera control**: drag to look around, rotate left/right buttons, auto-orbit toggle and a zoom slider.
- **Slideshow**: a Bootstrap carousel (fade effect, indicators, arrows, autoplay) hangs on the back wall.
- **Animations**: swaying plant, pulsing lamp light, drifting clouds in the window, floating slideshow icons and a cinematic orbit.
- **Themes**: Dusk, Sand, Forest and Neon. They change the wall, floor, sofa, sky and page background through CSS variables.
- **Fonts**: Poppins, Playfair Display, Space Grotesk and Caveat.
- **Lamp switch**: turns the lamp glow on and off.
- **Accessibility**: animations are disabled when the system asks for reduced motion.

## Structure

```
living-room-3d/
├── index.html   # markup, styles and scripts in one file
└── README.md
```

## Customise

- **Add a theme**: add a `[data-theme=name]` block with the same CSS variables, then add a button in the Theme dropdown.
- **Add furniture**: call `box(width, height, depth, x, yFromFloor, z, color)` in the script. The room is 600 x 360 x 600 px and the origin is the floor centre.
- **Add slides**: add another `.carousel-item` and indicator button inside the `#gallery` template.

## Technologies

HTML5, CSS3 (3D transforms, custom properties, keyframes), JavaScript ES6, Bootstrap 5.3 and Bootstrap Icons 1.11.

## Browser support

Current Chrome, Edge, Firefox and Safari.
