# Be Human — behmn.ai

Landing page for Be Human, a consulting company. It's a static site with no build step, ready for Netlify.

## Deploy to Netlify
1. In Netlify, choose **Add new site → Import an existing project** and pick this repo.
2. Leave the build command empty. The publish directory is `public` (already set in `netlify.toml`).
3. Deploy, then add the custom domain `behmn.ai` under **Domain management**.

The contact form uses Netlify Forms. Submissions appear under **Forms** in the Netlify dashboard once the site is deployed.

## Customizing
- Brand colors and fonts are CSS variables at the top of `public/styles.css`.
- Page copy is in `public/index.html`.
