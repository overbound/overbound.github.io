# Overbound Game Studio - Static Site

Static HTML version of [overboundstudio.com](https://overboundstudio.com), ready for GitHub Pages.

## Pages
- `index.html` — Home
- `games.html` — Games archive
- `sonic-time-twisted.html` — Sonic Time Twisted game page
- `no-more-robots.html` — No More Robots game page
- `blog.html` — Blog archive
- `blog-sonic-full-game-released.html` — Blog post
- `blog-release-date.html` — Blog post
- `blog-grand-opening.html` — Blog post
- `pixel-art-tutorials.html` — Pixel Art Tutorials
- `developer-logs.html` — Developer Logs
- `404.html` — 404 page

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `overboundstudio`)
2. Push this folder to it:
   ```
   git init
   git add .
   git commit -m "Initial static site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/overboundstudio.git
   git push -u origin main
   ```
3. Go to **Settings → Pages** in your repo
4. Set Source to **Deploy from a branch**, branch: `main`, folder: `/ (root)`
5. Your site will be live at `https://YOUR_USERNAME.github.io/overboundstudio/`

## Custom Domain (overboundstudio.com)

To use your custom domain:
1. In GitHub Pages settings, enter `overboundstudio.com` in the Custom Domain field
2. Add a `CNAME` file to this repo containing just: `overboundstudio.com`
3. Update your domain's DNS:
   - Add 4 A records pointing to GitHub's IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Or add a CNAME record: `www` → `YOUR_USERNAME.github.io`

## Images Note

Images currently load from `overboundstudio.com`. To fully self-host, download the images folder from your server and update the `src` paths in each HTML file.
