# LiquidEffect
Javascript Library for creating liquid effect on image and RGB effect on mouse direction.

## Demo
https://liquideffect.netlify.app/

# Dependencies
## NPM Package
```html
npm i pixi.js
npm i @pixi/filter-displacement
npm i @pixi/filter-rgb-split
```
## Browser
```html
<script src="https://cdn.jsdelivr.net/npm/pixi.js@5.3.3/dist/pixi.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/pixi-filters@2.6.1/dist/pixi-filters.js"></script>
<script src="<PATH_TO_FILE>/LiquidEffect.js"></script>
```

# Usage
## Vanilla JavaScript
```html
<script>
    new LiquidEffect({
        appendTo: "#main",
        image: './assets/images/image.jpg',
        displacementImage: "./assets/images/displacement_map.jpg",
        displacementScale: 1,
        speed: 1,
        intensityX: 1.5,
        intensityY: 1.5,
    });
</script>
```
## With Framework
```javascript
npm i liquideffect

import LiquidEffect from 'liquid-effect'

LiquidEffect({
    appendTo: "#main",
    image: './assets/images/image.jpg',
    displacementImage: "./assets/images/displacement_map.jpg",
    displacementScale: 1,
    speed: 1,
    intensityX: 1.5,
    intensityY: 1.5,
});
```

## Parameters

| Name                    | Type            | Description |
|-------------------------|-----------------|-------------|
|`appendTo`               | `Dom Element`   | Parent Element |
|`image`                  | `Image`         | Image to display|
|`displacementImage`      | `Image`         | Displacement Image |
|`displacementScale`      | `Float`         | Displacement Scale value 0.0 - 1.0 causing waves to be shorter or bigger |
|`speed`                  | `Float`         | Liquid effect wave speed |
|`intensityX`             | `Float`         | Liquid effect intensity on X-axis |
|`intensityY`             | `Float`         | Liquid effect intensity on Y-axis |
