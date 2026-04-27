# Bluestone PIM Labs Site Template

A single-file documentation site template for [Bluestone PIM Labs](https://labs.bluestonepim.com/) projects. Fork it to get a sidebar, dark mode, copyable markdown source, and consistent visual identity with other Labs projects: no build step, no dependencies.

## What you get

- Sticky header with logo, GitHub link, optional beta badge, and dark mode toggle
- Sidebar navigation with active section tracking
- Prose content written in Markdown inside a `<script type="text/plain">` block
- `[screenshot: file.webp]`, `[prompt: text]`, and `[reply: text]` shortcodes for rich documentation
- Changelog badge classes: `badge-new`, `badge-improved`, `badge-fixed`, `badge-note`
- "Copy page as Markdown" dropdown with "Open in Claude": lets readers share the docs with an LLM
- Anchor links on all headings
- Disclaimer banner matching the Labs visual standard
- Deploys to Vercel with no configuration beyond connecting the repo

## How to use

1. Fork this repo
2. Open `index.html` and search for `TODO`: each one marks something to update (title, description, GitHub URL, author name)
3. Replace the Markdown content inside `<script type="text/plain" id="md">` with your project's documentation
4. Update the sidebar and mobile nav links to match your section headings
5. Push to GitHub and connect to Vercel: set no build command, output directory is `.`

## Deploying to Vercel

Connect the repo in the Vercel dashboard. No build command needed. The included `vercel.json` sets `outputDirectory` to `.` so Vercel serves `index.html` from the repo root.

## Adding screenshots

Put images in a `/images/` folder and reference them in the Markdown:

```
[screenshot: your-image.webp]
```

If the file does not exist yet, a placeholder frame renders instead so you can write the docs before the screenshots are ready.

## Listing your project on [Bluestone PIM Labs](https://labs.bluestonepim.com/)

Once your project is live, open a pull request to [bspim-labs/bluestone-pim-labs](https://github.com/bspim-labs/bluestone-pim-labs) adding an entry to `projects.json`. See [CONTRIBUTING.md](https://github.com/bspim-labs/bluestone-pim-labs/blob/main/CONTRIBUTING.md) for the required fields.

## Part of [Bluestone PIM Labs](https://labs.bluestonepim.com/)

A community project by [Viktor Lövgren](https://www.linkedin.com/in/viktorlovgren/). Not an official Bluestone PIM product.
