# RPG Dialogue Portfolio

A tiny, dependency-free RPG-style interactive dialogue page.

## Features

- Character GIF at the top
- RPG dialogue UI at the bottom
- Clickable question choices
- Different reaction GIF for each answer
- Returns to the idle GIF when you go back to the question list
- Responsive on desktop and mobile
- Works directly on GitHub Pages

## Files

```text
ryu-rpg-dialogue/
├─ index.html
└─ assets/
   ├─ idle.gif
   ├─ reaction-awesome.gif
   ├─ reaction-make.gif
   └─ reaction-tokyo.gif
```

## Replace the character GIFs

Keep the same filenames, or edit the `gif` paths inside `index.html`.

Recommended GIF ratio: **16:9** or a transparent character centered in a 16:9 canvas.

## Publish with GitHub Pages

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.
4. The site will appear at:

   `https://tokyosaysryu.github.io/ryu-rpg-dialogue/`

## Edit the questions

Inside `index.html`, find the `dialogue` array and edit the question, answer, GIF path, and status label for each item.
