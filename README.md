# 2D Transform Animation

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/2d-transform-animation/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

Runnable recreation of the uploaded 15.4-second, 720 × 1280 screen recording.

## Screen content

The page title is **2D Transform Animation**. The video shows a black background, pink glowing title, bright blue outline around a two-column workspace, six dark preview cards on the left and a `CSS Source` panel on the right. Each card contains a cyan-to-purple gradient rounded square and a transform label.

The six examples, in the order shown:

1. Translate
2. Scale
3. Rotate
4. Skew
5. Matrix
6. Combined

Hover each card to see its transform. The CSS transition visible in the video is:

```css
.shape {
  transition:
    transform 0.6s
    cubic-bezier(0.34,
    1.56, 0.64, 1);
  will-change:
    transform;
}
```

The visible hover declarations include:

```css
.card:hover .shape {
  transform:
    translate(40px, -30px);
}
```

```css
.card:hover .shape {
  transform: scale(1.4);
}
```

```css
.card:hover .shape {
  transform: rotate(45deg);
}
```

```css
.card:hover .shape {
  transform: skew(-20deg, 10deg);
}
```

```css
.card:hover .shape {
  transform:
    translate(20px, 20px) rotate(45deg)
    scale(1.2);
}
```

The matrix-specific transform value is not legible in the supplied recording. This project uses `matrix(1, .2, .2, 1, 20, 12)` as a working illustrative reconstruction, not as a verified transcription.

## Run

1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Hover over each card to trigger its 2D transform.

No packages, JavaScript, build tools, external assets, or server are required.

## Files

- `index.html` — six preview cards and CSS source panel
- `style.css` — page styling and transform effects
- `README.md` — transcription notes and run instructions

## Fidelity note

The visible labels, transition declaration, and readable transform declarations are transcribed from the video. The complete page structure and supporting styles are recreated. The matrix value is explicitly an illustrative choice because its original value cannot be read from the recording.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
