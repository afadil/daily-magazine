# Daily Magazine

An HTML magazine published daily via GitHub Pages.

Live at: https://afadil.github.io/daily-magazine/

## Structure

```
index.html            # archive landing page (list of all issues)
issues/
  YYYY-MM-DD.html     # one file per day, permanent URL
```

## Daily workflow

1. Save today's HTML as `issues/YYYY-MM-DD.html`.
2. Open `index.html` and add a new `<li>` at the top of the `<ul class="issues">` list:
   ```html
   <li>
     <a href="issues/YYYY-MM-DD.html">Issue &mdash; Month D, YYYY</a>
     <span class="date">YYYY-MM-DD</span>
   </li>
   ```
3. Commit and push:
   ```sh
   git add . && git commit -m "Issue YYYY-MM-DD" && git push
   ```

Site updates within ~30 seconds.

## One-time setup (already done)

- Repo: https://github.com/afadil/daily-magazine
- GitHub Pages: Settings → Pages → Deploy from `main` / `/ (root)`
