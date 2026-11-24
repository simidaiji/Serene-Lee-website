# Serena Lee Photography

One-page personal site for freelance wedding and portrait photographer Serena Lee. Plain HTML and CSS, no build step.

## Structure

- `index.html` – the whole page (hero, portfolio grid, about, contact)
- `images/` – portfolio photos
- `vercel.json` – Vercel config (static deploy, security headers, image caching)

## Adding photos

Put the file in `images/`, then replace a placeholder `<div class="frame ...">` in `index.html` with:

```html
<img class="frame" src="images/your-photo.jpg" alt="Describe the photo">
```

Photos display at a 4:5 ratio. Use JPEGs about 1600px on the long edge.

## Preview locally

```sh
npx serve .
```

## Deploy on Vercel

1. In Vercel, choose **Add New → Project** and import this GitHub repo.
2. Leave Framework Preset as **Other**, with no build command and no output directory override.
3. Deploy. Every push to `main` redeploys automatically.

Or from the terminal: `npx vercel --prod`.
