# Samhain: History and Appalachian Traditions

A slide deck that runs in the browser. Everything (fonts, styles, scripts) lives in `index.html`, so it works hosted on GitHub Pages or opened straight off the hard drive with no internet.

## Presenting

| Key | Does |
| --- | --- |
| Space, →, ↓, Page Down, Enter | Next slide |
| Shift+Space, ←, ↑, Page Up, Backspace | Previous slide |
| Home / End | First / last slide |
| F | Fullscreen on/off |

Clicking works too: the left third of the screen goes back, anywhere else goes forward. Presentation clickers work out of the box. On phones and tablets, swipe.

The slide number is kept in the address bar (`#12`), so refreshing keeps your place.

## Adding photos

Each photo on a slide points to a file in `images/`. If that file is missing, the slide shows a dashed placeholder with the file name it expects, so replacing a photo is just a matter of saving the new one under the same name.

To put a photo on any other slide, add this inside that slide's `<section>`:

```html
<figure class="photo">
  <img src="images/your-photo.jpg" alt="What the photo shows">
  <figcaption class="missing-note">Photo goes here<span>images/your-photo.jpg</span></figcaption>
</figure>
```

For a full-height photo, on a slide by itself or beside text, use `class="photo solo"`. To credit a photo, add `<figcaption class="credit">Credit line</figcaption>` before the `missing-note` line.

## Unfinished sections

Anything still being written shows "Content to come." Search `index.html` for `class="todo"` to find them.

## Hosting on GitHub Pages

1. Push this folder to a repo (with `index.html` at the root).
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → `main` / `root`.
3. After a minute it's live at https://bstaack.github.io/samhain/

Keep a downloaded copy on the presenting computer as a backup. Double-clicking `index.html` works without wifi.
