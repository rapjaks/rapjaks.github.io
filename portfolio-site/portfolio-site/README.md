# Portfolio site

A single-page site: `index.html` (all styles and scripts included) plus
`assets/resume.pdf` for the download link.

## Put it on GitHub Pages

1. On GitHub, create a new repository. Name it `your-username.github.io`
   (using your actual GitHub username) if you want it at the root of your
   GitHub domain — any other name works too, it'll just live at
   `your-username.github.io/repo-name`.
2. Upload `index.html` and the `assets` folder to the repo (drag-and-drop
   on the repo's "Add file → Upload files" page works fine, or use git).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment," set **Source** to "Deploy from a branch,"
   branch `main`, folder `/ (root)`. Save.
5. GitHub gives you a URL (something like `https://your-username.github.io`)
   — it can take a minute or two to go live the first time.

## Custom domain (optional)

If you buy a domain later, add it under **Settings → Pages → Custom domain**
and follow GitHub's DNS instructions there.

## Adding real projects

Open `index.html` and find the `const projects = [ ... ]` array near the
bottom, inside the `<script>` tag. Each object is one card — duplicate one,
fill in your own `title`, `tag`, `blurb`, `overview`, `process`,
`requirements`, and `user` fields, and it'll appear in the grid
automatically. The two "Project title" placeholders are there to copy.

The **Orbital Habitat Walkthrough** card is already set up for your 3D
space station simulator — once you've exported a web build from Unity or
Godot, that's the project to embed it in (an `<iframe>` or a WebGL canvas
dropped into the modal, or its own page linked from the card, both work).
