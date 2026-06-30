# King Panda Studio — website files

This folder is your complete, editable website. Put **everything in this folder** into your
GitHub repo (keep the structure exactly as-is) and enable GitHub Pages.

## Files in here
- `index.html` ........ the website (open this / it's the homepage)
- `support.js` ........ the engine that renders the page — don't edit, just keep it next to index.html
- `uploads/` .......... ALL your images live here
- `.nojekyll` ......... an empty file that tells GitHub to serve the page untouched (don't delete it)

## How to deploy to GitHub
1. Upload the contents of this folder to your repo (so `index.html`, `support.js`, `uploads/`,
   and `.nojekyll` all sit in the repo root).
2. Repo → Settings → Pages → Source = your branch (main) / root folder → Save.
3. Wait ~1 minute, then open https://<your-username>.github.io/<repo-name>/

Your site needs an internet connection to load fonts and the rendering engine — that's normal and works fine on GitHub Pages.

---

## HOW TO EDIT MEDIA

### Swap a picture (easiest)
Every image is a real file inside `uploads/`. To replace one, just put your new image in
`uploads/` using the SAME filename. For example, to change the Nullified cover, replace
`uploads/proj_nullified.png` with your new image (keep the name `proj_nullified.png`).

The project covers are:
- uploads/proj_nullified.png      (Nullified)
- uploads/proj_aetherforge.png    (AetherForge)
- uploads/proj_manawars.png       (Mana Wars)
- uploads/proj_dungeondivers.png  (Dungeon Divers)
- uploads/proj_codexrift.png      (Codex Rift)
- uploads/proj_accused.png        (Occulos: The Accused)

Team photos: uploads/team_ryan.jpg, team_nathan.jpg, team_brayden.jpg, team_group.jpg
Logo: uploads/kps_logo.png

### Point an image at a different file
Open `index.html` and search for `img:'uploads/`. Each project / team member has a line like:

    img:'uploads/proj_nullified.png',

Change the filename in the quotes to any file you've added to `uploads/`.

### Add a brand-new project
In `index.html`, find the block that starts with `return [` (around the project list). Copy one
existing `{ id:'...', title:'...', ... }` block, paste it as a new entry, and edit the title,
text, and `img:` path. Add its image to `uploads/`.

### Links (Discord, YouTube, social, "Get it")
Most buttons are currently placeholders. In `index.html` search for `href="#"` and replace `#`
with your real URL, e.g. `href="https://youtube.com/@yourchannel"`. The "Join Discord" and
social buttons can be wired the same way — ask and I can set real links for you.

---

Tip: editing raw code by hand is fiddly. The easiest path is to tell me what to change
("swap the team photo", "add this YouTube link", "new project called X") and I'll update the
files and hand you a fresh copy.
