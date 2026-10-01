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

The Tipton-Haynes slide already looks for `images/tipton-haynes.jpg`. Drop the photo in with that exact name and it shows up. Until then the slide shows a dashed placeholder.

To put a photo on any other slide, add this inside that slide's `<section>`:

```html
<figure class="photo">
  <img src="images/your-photo.jpg" alt="What the photo shows">
  <figcaption class="missing-note">Photo goes here<span>images/your-photo.jpg</span></figcaption>
</figure>
```

## Unfinished sections

Anything still being written shows "Content to come." Search `index.html` for `class="todo"` to find them.

## Hosting on GitHub Pages

1. Push this folder to a repo (with `index.html` at the root).
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → `main` / `root`.
3. After a minute it's live at `https://<username>.github.io/<repo-name>/`.

Keep a downloaded copy on the presenting computer as a backup. Double-clicking `index.html` works without wifi.
