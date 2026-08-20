# RPG Dialogue Portfolio

A GitHub Pages-ready interactive RPG dialogue interface inspired by a retro pixel-game UI.

## Current layout

- Logical canvas: **1420 × 610 px**
- Automatically scales down to fit smaller browser windows while preserving the 1420 × 610 composition
- Google Font: **Pixelify Sans**
- Dynamic Tokyo date header using the `Asia/Tokyo` timezone
- Pixel-style left navigation rail with external links
- Swappable background layer behind the character
- Character reaction GIF switches per question
- Swipe transition on dialogue/navigation interactions
- Paginated answers with a next/reset control
- Four interview questions fixed in the bottom response section

## Files

```text
ryu-rpg-dialogue/
├─ index.html
└─ assets/
   ├─ background.gif
   ├─ idle.gif
   ├─ reaction-awesome.gif
   ├─ reaction-make.gif
   ├─ reaction-tokyo.gif
   └─ reaction-about.gif
```

## Replace the background

Replace `assets/background.gif` with your own GIF using the same filename.

For a PNG, upload something such as `assets/background.png`, then change this line in `index.html`:

```html
<img class="scene-bg" src="assets/background.gif" ... />
```

to:

```html
<img class="scene-bg" src="assets/background.png" ... />
```

## Replace character reactions

Keep the existing GIF filenames or edit each `gif` path in the `dialogue` array inside `index.html`.

## External links

Edit the `externalLinks` array near the bottom of `index.html`:

```js
const externalLinks = [
  { label: "Portfolio", glyph: "WEB", href: "https://example.com" }
];
```

## Questions and answers

Edit the `dialogue` array. Each answer is stored as a `pages` array. Add another string when you want the **Next** button to continue the answer on a new page.

## GitHub Pages

Publish from:

- Branch: `main`
- Folder: `/ (root)`

Live URL:

`https://tokyosaysryu.github.io/ryu-rpg-dialogue/`
